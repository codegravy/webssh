# ROADMAP 

Initial planning goals for WebSSH are listed below. (in no particular order)

[ ] SSH server bridge. 
    [ ] Should accept encrypted websocket/webRTC connections and attempt to connect to an existing ssh server.
     *  Not sure how much work we want/need the server to do, especially if we eventually move to local TCP instead.
    [ ] May eventually replace with local TCP socket.  Follow https://bugzilla.mozilla.org/show_bug.cgi?id=1247628 for mor information.
    [ ] websockify may work as well.  Seems to be a 1-to-1 connection to a tcp server.
[ ] SSH client library.
    [ ] Pure JavaScript or WebAssembly client library to interface with hterm or the like.
     *  https://pijul.org/thrussh/ may be good through wasm.
     *  How to access private ssh key? Or do we just generate it locally and store it in-browser somehow?
[ ] HTerm compatablilty.
     *  How easy is it to link the SSH Client io to HTerm, seems it may be easier that expected, but needs more research.

