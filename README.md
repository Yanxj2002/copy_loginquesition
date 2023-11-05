# copy_loginquesition 不要让某些网站强奸你(登录复制)

document.querySelector("main").querySelectorAll("*").forEach(e => {
  const listeners = getEventListeners(e)
  if (listeners && listeners.copy) {
    listeners.copy.forEach(l => e.removeEventListener("copy", l.listener))
  }
})

某些需要登录甚至付费才能复制的网站，都给我爬开，都2023年了，道德绑架你妈呢
