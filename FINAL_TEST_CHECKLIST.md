# 🧪 FINAL TEST CHECKLIST - Tam Thái Tử v1.0.0

**Test Date**: 2024-11-03 00:33  
**Server**: http://localhost:57434

---

## ✅ CRITICAL FIXES VERIFIED

### 1. Bug Fixes
- [x] `ErrorLog` → `ErrLog` (line 144, 1992, 2083)
- [x] `BUILD_INFO` → `BI` (line 2018, 2020)
- [x] Settings panel drag không bị "bay lên"
- [x] All variable names minified correctly

---

## 🎮 CORE GAME FEATURES

### Basic Functionality
- [ ] **Initial Load**: Page loads without console errors
- [ ] **Greeting Popup**: Shows on first visit with music options
- [ ] **Mode Selection**: Shows 5 modes (Play, Teach, Learn, Challenge, Sandbox)
- [ ] **Disk Movement**: 
  - [ ] Click disk to pick up
  - [ ] Click pole to place
  - [ ] Drag & drop works
  - [ ] Invalid moves show error popup
- [ ] **Move Counter**: Updates correctly
- [ ] **Timer**: Starts and updates
- [ ] **Progress Bar**: Updates for n≤8 disks

### Game Modes

#### 🎯 Play Mode
- [ ] Start with 3-12 disks
- [ ] Complete game shows correct popup (Perfect/Good/Success)
- [ ] Best score saves and displays
- [ ] Confetti animation on win
- [ ] Win sound plays

#### 📚 Teach Mode  
- [ ] Auto-advance through optimal solution
- [ ] Hint text shows: "Di chuyển từ Cọc X → Y" (bold, gradient)
- [ ] Can pause/resume
- [ ] Poles highlight correctly
- [ ] Completion popup shows

#### 🧠 Learn Mode
- [ ] Panel appears (right side on desktop)
- [ ] **Draggable**: Can drag by header
- [ ] **Minimize**: Click − to collapse
- [ ] **Close**: Click × to close
- [ ] Algorithm visualization shows
- [ ] Step-by-step controls work
- [ ] Pseudocode highlights correctly

#### ⚔️ Challenge Mode
- [ ] Difficulty selection (Easy/Medium/Hard)
- [ ] Timer countdown works
- [ ] Move limit enforced
- [ ] Success shows challenge win popup
- [ ] Failure shows loser popup
- [ ] Time runs out triggers failure

#### 🔬 Sandbox Mode
- [ ] Setup popup opens
- [ ] Configure disks (2-8)
- [ ] Configure poles (3-6)
- [ ] Rule options work:
  - [ ] Classic
  - [ ] Adjacent only
  - [ ] No direct
- [ ] Start position options:
  - [ ] Classic (all on pole 1)
  - [ ] Spread
  - [ ] Last pole
- [ ] Target options work
- [ ] Frame-Stewart info shows for 4-5 poles
- [ ] **Sandbox Win Popup** (🚀🧪) shows for non-classic rules
- [ ] Confetti purple for sandbox

---

## 🎨 UI/UX FEATURES

### Theme System
- [ ] Classic theme works
- [ ] Dark Cozy theme works (background, colors, shadows)
- [ ] Burger, Rescue, Neon themes work
- [ ] Theme persists on reload
- [ ] Achievement "Collector" unlocks on theme change

### Controls
- [ ] Reset button works
- [ ] Undo button works (enabled when moves exist)
- [ ] Auto-solve button works
- [ ] Speed slider changes animation speed
- [ ] Number input changes disk count

### Layout
- [ ] **Full-width**: Game fills screen (max 1400px)
- [ ] No white space on sides
- [ ] Responsive on mobile
- [ ] All popups center correctly

---

## 🏆 ACHIEVEMENT SYSTEM

### Basic Achievements
- [ ] "Tân Binh" (Rookie) - Default
- [ ] "Nhà Thực Hành" - Complete Play mode
- [ ] "Học Sinh" - Complete Teach mode
- [ ] "Học Giả" - Complete Learn mode
- [ ] "Nhà Tiên Phong" - Complete Sandbox
- [ ] "Nhà Sưu Tầm" - Change theme

### Challenge Achievements  
- [ ] "Thách Thức" - Win any challenge
- [ ] "Chấp Nhận Thách Thức" - Start challenge

### Advanced Achievements
- [ ] "Bất Bại" - 10+ disks optimal, no undo
- [ ] "Hoàn Mỹ Tuyệt Đối" - 12 disks optimal
- [ ] "Huyền Thoại Tốc Độ" - 8+ disks in 2min
- [ ] "Tháp Chủ" - Unlock all others

### Title System
- [ ] Click title badge opens achievements popup
- [ ] Can select different titles
- [ ] Selected title displays with checkmark
- [ ] Title persists on reload

---

## 🔊 AUDIO SYSTEM

### BGM (Background Music)
- [ ] Plays on first visit if user clicks "Có, bật nhạc"
- [ ] **Auto-plays on return visits** if enabled
- [ ] Checkbox ☑ Âm toggles BGM
- [ ] Custom BGM upload works
- [ ] Custom BGM persists

### Sound Effects
- [ ] Pickup sound on disk grab
- [ ] Drop sound on disk place
- [ ] Error sound on invalid move
- [ ] Win sound on completion
- [ ] Fireworks sound with confetti

### Audio Blocked Notice
- [ ] **Browser blocks autoplay** → Shows hint:
  ```
  🔇 Âm thanh bị chặn - Click checkbox ☑ Âm để bật lại
  ```
- [ ] Click retry checkbox plays BGM
- [ ] Works in Chrome/Firefox/Edge

---

## 🖼️ CUSTOM BACKGROUND

### Upload Feature
- [ ] Settings → Background section visible
- [ ] Upload image (<5MB) works
- [ ] Status changes to "Đã tùy chỉnh"
- [ ] Background displays correctly
- [ ] **Opacity slider** (0-100%) works
- [ ] Persists on reload

### Reset
- [ ] "Khôi phục Mặc định" clears background
- [ ] Status resets to "Mặc định"

---

## ⚙️ SETTINGS PANEL

### New Design
- [ ] **Opens as draggable panel** (not fullscreen popup)
- [ ] **Size**: ~480px wide, 85vh max height
- [ ] **Header**: Blue gradient with ⚙️ Cài đặt title
- [ ] **Minimize button** (−): Collapses content
- [ ] **Close button** (×): Closes panel

### Draggable
- [ ] **Drag by header**: Panel moves
- [ ] **No jump/fly**: Smooth movement
- [ ] **Boundary check**: Can't drag off-screen
- [ ] **Ignores buttons**: Minimize/Close don't trigger drag
- [ ] **Touch support**: Works on mobile

### Sections

#### 🎨 Background
- [ ] Image upload input
- [ ] Opacity slider with value display
- [ ] Status shows custom/default

#### 🎵 Audio  
- [ ] BGM upload
- [ ] Pickup sound upload
- [ ] Drop sound upload
- [ ] Win sound upload
- [ ] Each shows upload status

#### 🗑️ Cache Manager
- [ ] **"xóa bộ nhớ đệm"** button:
  - [ ] Shows confirm
  - [ ] Clears custom audio/background
  - [ ] Keeps achievements/scores
  - [ ] Shows success message
  
- [ ] **"XÓA TOÀN BỘ DỮ LIỆU"** button (RED):
  - [ ] Shows 2 confirms with warnings
  - [ ] Clears EVERYTHING
  - [ ] Reloads page
  
- [ ] Warning text displays

#### Footer
- [ ] "Khôi phục Mặc định" button works

---

## 🌓 DARK MODE

- [ ] Settings panel dark theme
- [ ] Settings content readable
- [ ] Setting items dark background
- [ ] Border colors adjusted
- [ ] All text readable

---

## 💾 DATA PERSISTENCE

### LocalStorage Keys
- [ ] `hanoi_game_state_v3` - Game state
- [ ] `hanoi_unlocked_achievements` - Achievements
- [ ] `hanoi_selected_title` - Selected title
- [ ] `hanoi_best_v2_{n}_disks` - Best scores
- [ ] `customBGM`, `customPickup`, etc - Custom audio
- [ ] `customBackground`, `bgOpacity` - Custom bg
- [ ] `hanoi_seen_greeting` - Greeting flag

### Persistence Tests
- [ ] Complete game → Reload → State restored
- [ ] Change theme → Reload → Theme kept
- [ ] Unlock achievement → Reload → Still unlocked
- [ ] Upload custom audio → Reload → Still custom
- [ ] Upload background → Reload → Still there

---

## 📱 RESPONSIVE DESIGN

### Desktop (>768px)
- [ ] Full layout with all features
- [ ] Learn panel on right side
- [ ] Settings panel centered
- [ ] Optimal spacing

### Tablet (500-768px)
- [ ] Layout adapts
- [ ] Buttons stack appropriately
- [ ] Popups fit screen

### Mobile (<500px)
- [ ] All features accessible
- [ ] Touch controls work
- [ ] Learn panel fixed at bottom
- [ ] Settings panel responsive
- [ ] Font sizes readable

---

## 🐛 ERROR HANDLING

### Console Checks
- [ ] No JavaScript errors on load
- [ ] No errors during gameplay
- [ ] No errors on mode switch
- [ ] No errors on achievement unlock
- [ ] No errors on audio play (except blocked)

### Error Popup
- [ ] Shows on invalid move
- [ ] Message clear
- [ ] "Hiểu rồi" button closes it

### Debug Tools
- [ ] `HanoiDebug.errors()` returns error log
- [ ] `HanoiDebug.state()` returns game state
- [ ] `HanoiDebug.resetAch()` resets achievements
- [ ] `HanoiDebug.info()` returns build info

---

## 🎯 SPECIAL SCENARIOS

### Edge Cases
- [ ] Auto-solve after making moves
- [ ] Undo after auto-solve
- [ ] Switch modes mid-game
- [ ] Upload very large file (>5MB rejected)
- [ ] Upload invalid file type
- [ ] Challenge timer reaches 0
- [ ] Sandbox with max config (8 disks, 6 poles)

### Multi-Session
- [ ] Play → Close browser → Reopen → Resume
- [ ] Unlock 10 achievements → All display correctly
- [ ] Change settings → Close → Reopen → Settings kept

---

## 📊 PERFORMANCE

- [ ] Page loads in <3 seconds
- [ ] Animations smooth (60fps)
- [ ] No lag with 12 disks
- [ ] Drag operations smooth
- [ ] Audio plays without delay

---

## ✅ FINAL CHECKLIST

### Code Quality
- [x] All comments cleaned (max 2-3 words)
- [x] Variable names minified
- [x] No undefined references
- [x] All functions defined
- [x] All IDs match HTML

### Files Ready
- [x] `index.html` - Optimized
- [x] `ap2.js` - Minified & clean
- [x] `stylesen1.css` - Optimized
- [x] All assets present

### Browser Compatibility
- [ ] Chrome - All features work
- [ ] Firefox - All features work
- [ ] Edge - All features work
- [ ] Safari - All features work
- [ ] Mobile Chrome - All features work
- [ ] Mobile Safari - All features work

---

## 🚀 DEPLOYMENT READY?

- [ ] All critical tests pass
- [ ] No console errors
- [ ] All features functional
- [ ] Performance acceptable
- [ ] Responsive on all devices
- [ ] Data persists correctly

**Status**: 🟡 IN TESTING

---

**Test by clicking through features in browser preview!**  
**Server**: http://localhost:57434
