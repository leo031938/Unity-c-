using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class bottom : MonoBehaviour
{
    // Start is called before the first frame update
    private void OnCollisionEnter2D(Collision2D other)
    {

        if (other.gameObject.CompareTag("player"))
        {
            player.dead = true;
            Destroy(other.gameObject);
        }
        else if (other.gameObject.CompareTag("player2"))
        {
            player2.dead = true;
            Destroy(other.gameObject);
        }
    }
}
