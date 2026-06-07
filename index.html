<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>形婚网 - 形婚信息平台</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; background: #f0f2f5; }
    .header { background: #fff; padding: 16px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); position: sticky; top: 0; z-index: 100; }
    .header h1 { font-size: 20px; color: #1a73e8; text-align: center; }
    .tabs { display: flex; background: #fff; border-bottom: 1px solid #e0e0e0; overflow-x: auto; }
    .tab { flex: 1; min-width: 100px; padding: 14px 12px; text-align: center; font-size: 14px; color: #666; cursor: pointer; border-bottom: 3px solid transparent; transition: all 0.2s; white-space: nowrap; }
    .tab.active { color: #1a73e8; border-bottom-color: #1a73e8; font-weight: 600; }
    .cards { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 16px; padding: 16px; }
    .card { background: #fff; border-radius: 16px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.08); transition: transform 0.2s; }
    .card:hover { transform: translateY(-4px); }
    .card-header { position: relative; }
    .card-avatar { width: 100%; height: 180px; object-fit: cover; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; }
    .card-avatar img { width: 80px; height: 80px; border-radius: 50%; border: 3px solid #fff; box-shadow: 0 4px 12px rgba(0,0,0,0.15); }
    .card-badge { position: absolute; top: 12px; left: 12px; background: #1a73e8; color: #fff; padding: 4px 10px; border-radius: 20px; font-size: 12px; font-weight: 600; }
    .card-badge.female { background: #e91e63; }
    .card-online { position: absolute; top: 12px; right: 12px; width: 12px; height: 12px; background: #34a853; border-radius: 50%; border: 2px solid #fff; }
    .card-body { padding: 16px; }
    .card-name { font-size: 18px; font-weight: 700; color: #333; margin-bottom: 8px; display: flex; align-items: center; gap: 8px; }
    .card-name .verified { color: #1a73e8; font-size: 14px; }
    .card-tags { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 12px; }
    .tag { background: #e8f0fe; color: #1a73e8; padding: 4px 10px; border-radius: 6px; font-size: 12px; }
    .tag.female { background: #fce4ec; color: #c2185b; }
    .card-info { font-size: 13px; color: #666; line-height: 1.6; }
    .card-info div { margin-bottom: 4px; }
    .card-footer { padding: 12px 16px; border-top: 1px solid #f0f0f0; display: flex; justify-content: space-between; align-items: center; }
    .card-time { font-size: 12px; color: #999; }
    .card-btn { background: #1a73e8; color: #fff; border: none; padding: 8px 20px; border-radius: 20px; font-size: 13px; font-weight: 600; cursor: pointer; }
    .card-btn:hover { background: #1557b0; }
    .fab { position: fixed; bottom: 24px; right: 24px; width: 56px; height: 56px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: #fff; border: none; border-radius: 50%; font-size: 28px; box-shadow: 0 4px 16px rgba(102, 126, 234, 0.5); cursor: pointer; z-index: 1000; transition: transform 0.2s, box-shadow 0.2s; }
    .fab:hover { transform: scale(1.1); box-shadow: 0 6px 20px rgba(102, 126, 234, 0.6); }
    .modal { position: fixed; top: 0; left: 0; right: 0; bottom: 0; background: rgba(0,0,0,0.5); display: none; align-items: center; justify-content: center; z-index: 2000; padding: 20px; }
    .modal.active { display: flex; }
    .modal-content { background: #fff; border-radius: 20px; width: 100%; max-width: 500px; max-height: 90vh; overflow-y: auto; animation: slideUp 0.3s ease; }
    @keyframes slideUp { from { transform: translateY(50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
    .modal-header { padding: 20px; border-bottom: 1px solid #eee; display: flex; justify-content: space-between; align-items: center; }
    .modal-header h2 { font-size: 18px; color: #333; }
    .modal-close { background: none; border: none; font-size: 24px; color: #999; cursor: pointer; padding: 0; width: 32px; height: 32px; display: flex; align-items: center; justify-content: center; }
    .modal-close:hover { color: #333; }
    .modal-body { padding: 20px; }
    .form-group { margin-bottom: 16px; }
    .form-group label { display: block; margin-bottom: 6px; font-size: 14px; color: #555; font-weight: 500; }
    .form-group input, .form-group select, .form-group textarea { width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 10px; font-size: 14px; transition: border-color 0.2s; }
    .form-group input:focus, .form-group select:focus, .form-group textarea:focus { outline: none; border-color: #1a73e8; }
    .form-row { display: flex; gap: 12px; }
    .form-row .form-group { flex: 1; }
    .modal-footer { padding: 16px 20px; border-top: 1px solid #eee; display: flex; gap: 12px; }
    .modal-footer button { flex: 1; padding: 14px; border-radius: 10px; font-size: 15px; font-weight: 600; cursor: pointer; transition: all 0.2s; }
    .btn-cancel { background: #f5f5f5; color: #666; border: 1px solid #ddd; }
    .btn-cancel:hover { background: #e8e8e8; }
    .btn-submit { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: #fff; border: none; }
    .btn-submit:hover { opacity: 0.9; }
    .empty { text-align: center; padding: 60px 20px; color: #999; }
    .empty-icon { font-size: 64px; margin-bottom: 16px; }
    .search-bar { padding: 12px 16px; background: #fff; border-bottom: 1px solid #eee; }
    .search-input { width: 100%; padding: 10px 16px; border: 1px solid #ddd; border-radius: 25px; font-size: 14px; background: #f5f5f5; }
    .search-input:focus { outline: none; background: #fff; border-color: #1a73e8; }
    .counter { padding: 12px 16px; background: #e8f0fe; color: #1a73e8; text-align: center; font-size: 14px; }
    .counter span { font-weight: 700; }
  </style>
</head>
<body>
  <div class="header">
    <h1>形婚网</h1>
  </div>
  
  <div class="tabs">
    <div class="tab active" data-filter="all">全部</div>
    <div class="tab" data-filter="male">男士</div>
    <div class="tab" data-filter="female">女士</div>
  </div>
  
  <div class="search-bar">
    <input type="text" class="search-input" placeholder="搜索姓名、地区..." id="searchInput">
  </div>
  
  <div class="counter">当前共有 <span id="counter">0</span> 位会员</div>
  
  <div class="cards" id="cards">
    <div class="empty">
      <div class="empty-icon">📋</div>
      <p>暂无会员信息</p>
      <p style="font-size:13px;margin-top:8px;">点击右下角"+"按钮添加</p>
    </div>
  </div>
  
  <button class="fab" id="fabBtn" title="添加新会员">+</button>
  
  <div class="modal" id="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>登记档案</h2>
        <button class="modal-close" id="closeModal">×</button>
      </div>
      <div class="modal-body">
        <form id="memberForm">
          <div class="form-group">
            <label>姓名 *</label>
            <input type="text" id="name" required placeholder="请输入姓名">
          </div>
          <div class="form-row">
            <div class="form-group">
              <label>性别 *</label>
              <select id="gender" required>
                <option value="male">男</option>
                <option value="female">女</option>
              </select>
            </div>
            <div class="form-group">
              <label>年龄 *</label>
              <input type="number" id="age" required min="18" max="60" placeholder="24">
            </div>
          </div>
          <div class="form-row">
            <div class="form-group">
              <label>身高(cm) *</label>
              <input type="number" id="height" required min="150" max="200" placeholder="170">
            </div>
            <div class="form-group">
              <label>所在城市 *</label>
              <select id="city" required>
                <option value="">请选择</option>
                <option value="北京">北京</option>
                <option value="上海">上海</option>
                <option value="广州">广州</option>
                <option value="深圳">深圳</option>
                <option value="杭州">杭州</option>
                <option value="南京">南京</option>
                <option value="武汉">武汉</option>
                <option value="成都">成都</option>
                <option value="重庆">重庆</option>
                <option value="西安">西安</option>
                <option value="苏州">苏州</option>
                <option value="天津">天津</option>
                <option value="长沙">长沙</option>
                <option value="郑州">郑州</option>
                <option value="其他">其他</option>
              </select>
            </div>
          </div>
          <div class="form-group">
            <label>形婚目的 *</label>
            <select id="purpose" required>
              <option value="">请选择</option>
              <option value="形婚">形婚</option>
              <option value="恋爱">恋爱</option>
              <option value="结婚">结婚</option>
              <option value="朋友">朋友</option>
              <option value="形婚/恋爱">形婚/恋爱</option>
            </select>
          </div>
          <div class="form-group">
            <label>个人简介</label>
            <textarea id="intro" rows="3" placeholder="简单介绍一下自己..."></textarea>
          </div>
        </form>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn-cancel" id="cancelBtn">取消</button>
        <button type="button" class="btn-submit" id="submitBtn">提交登记</button>
      </div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = 'xinghun_profiles';
    const modal = document.getElementById('modal');
    const fabBtn = document.getElementById('fabBtn');
    const closeModal = document.getElementById('closeModal');
    const cancelBtn = document.getElementById('cancelBtn');
    const submitBtn = document.getElementById('submitBtn');
    const memberForm = document.getElementById('memberForm');
    const searchInput = document.getElementById('searchInput');
    let currentFilter = 'all';
    let profiles = JSON.parse(localStorage.getItem(STORAGE_KEY) || '[]');
    
    function render() {
      const cards = document.getElementById('cards');
      const counter = document.getElementById('counter');
      let filtered = profiles;
      
      if (currentFilter !== 'all') {
        filtered = profiles.filter(p => p.gender === currentFilter);
      }
      
      const search = searchInput.value.toLowerCase();
      if (search) {
        filtered = filtered.filter(p => 
          p.name.toLowerCase().includes(search) || 
          p.city.toLowerCase().includes(search)
        );
      }
      
      counter.textContent = filtered.length;
      
      if (filtered.length === 0) {
        cards.innerHTML = '<div class="empty"><div class="empty-icon">📋</div><p>暂无会员信息</p><p style="font-size:13px;margin-top:8px;">点击右下角"+"按钮添加</p></div>';
        return;
      }
      
      cards.innerHTML = filtered.map(p => `
        <div class="card">
          <div class="card-header">
            <div class="card-avatar" style="background: ${p.gender === 'male' ? 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)' : 'linear-gradient(135deg, #f093fb 0%, #f5576c 100%)'}">
              <img src="${p.avatar || 'https://api.dicebear.com/7.x/avataaars/svg?seed=' + p.id}" alt="${p.name}">
            </div>
            <div class="card-badge ${p.gender === 'female' ? 'female' : ''}">${p.gender === 'male' ? '男' : '女'}</div>
            ${p.online ? '<div class="card-online"></div>' : ''}
          </div>
          <div class="card-body">
            <div class="card-name">${p.name} ${p.verified ? '<span class="verified">✓</span>' : ''}</div>
            <div class="card-tags">
              <span class="tag ${p.gender === 'female' ? 'female' : ''}">${p.age}岁</span>
              <span class="tag ${p.gender === 'female' ? 'female' : ''}">${p.height}cm</span>
              <span class="tag ${p.gender === 'female' ? 'female' : ''}">${p.city}</span>
            </div>
            <div class="card-info">
              <div>📌 ${p.purpose}</div>
              <div>${p.intro || '暂无简介'}</div>
            </div>
          </div>
          <div class="card-footer">
            <span class="card-time">${p.lastActive ? new Date(p.lastActive).toLocaleDateString('zh-CN') : ''}</span>
            <button class="card-btn">联系TA</button>
          </div>
        </div>
      `).join('');
    }
    
    fabBtn.onclick = () => modal.classList.add('active');
    closeModal.onclick = () => modal.classList.remove('active');
    cancelBtn.onclick = () => modal.classList.remove('active');
    
    modal.onclick = (e) => { if (e.target === modal) modal.classList.remove('active'); };
    
    submitBtn.onclick = () => {
      if (!memberForm.checkValidity()) {
        memberForm.reportValidity();
        return;
      }
      
      const profile = {
        id: 'u' + Date.now(),
        name: document.getElementById('name').value,
        gender: document.getElementById('gender').value,
        age: parseInt(document.getElementById('age').value),
        height: parseInt(document.getElementById('height').value),
        city: document.getElementById('city').value,
        purpose: document.getElementById('purpose').value,
        intro: document.getElementById('intro').value,
        avatar: 'https://api.dicebear.com/7.x/avataaars/svg?seed=' + Date.now(),
        verified: false,
        online: true,
        lastActive: new Date().toISOString()
      };
      
      profiles.push(profile);
      localStorage.setItem(STORAGE_KEY, JSON.stringify(profiles));
      
      memberForm.reset();
      modal.classList.remove('active');
      render();
    };
    
    document.querySelectorAll('.tab').forEach(tab => {
      tab.onclick = () => {
        document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
        tab.classList.add('active');
        currentFilter = tab.dataset.filter;
        render();
      };
    });
    
    searchInput.oninput = render;
    
    render();
  </script>
</body>
</html>
