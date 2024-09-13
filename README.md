import java.util.LinkedList;

public class PlayList {
	
	static int size=3;

    public static void main(String[] args) {
       
        
        
        LinkedList songlist=new LinkedList();
        
        songlist.add("s1");
        songlist.add("s2");
        songlist.add("s3");
        
        
       
        System.out.println(songlist);
        
        songlist.add("s4");      
        System.out.println(removeFirstSong(songlist));
        
        songlist.add("s2");      
        System.out.println(removeFirstSong(songlist));
        
        
        songlist.add("s1");      
        System.out.println(removeFirstSong(songlist));
   }

    
    static LinkedList  removeFirstSong(LinkedList songlist){
        
        
        if(size<songlist.size())
        songlist.removeFirst();
        
        
        
        return songlist;
        
    }

}
