use Test;
use Cro;
use Cro::TLS;

ok Cro::TLS::Listener ~~ Cro::Source, 'TLS listener is a source';
ok Cro::TLS::Listener.produces ~~ Cro::TLS::ServerConnection, 'TLS listener produces connections';
ok Cro::TLS::ServerConnection ~~ Cro::Connection, 'TLS connection is a connection';
ok Cro::TLS::ServerConnection ~~ Cro::Replyable, 'TLS connection is replyable';
ok Cro::TLS::ServerConnection.produces ~~ Cro::TCP::Message, 'TLS connection produces TCP messages';
ok Cro::TLS::Connector ~~ Cro::Connector, 'TLS connector is a connector';
ok Cro::TLS::Connector.consumes ~~ Cro::TCP::Message, 'TLS connector consumes TCP messages';
ok Cro::TLS::Connector.produces ~~ Cro::TCP::Message, 'TLS connector produces TCP messages';

done-testing;
