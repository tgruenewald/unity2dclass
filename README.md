# unity2dclass
Materials for Unity 2D Platformer class

Fully complete code:  https://github.com/tgruenewald/2dclass_day1

My site:  www.daretogame.net

Ludum Dare:  www.ldjam.com   


# Flip


	private bool facingRight = true;
		if (move > 0 && !facingRight)
        {
            Flip();
        }
        else if (move < 0 && facingRight)
        {
            Flip();
        }



    void Flip()
    {
        //Debug.Log("switching...");
        facingRight = !facingRight;
        Vector3 theScale = transform.localScale;
        theScale.x *= -1;
        transform.localScale = theScale;
    }	
