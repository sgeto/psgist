��

### NAME

New-Gist

    

### SYNOPSIS

Publishes Github Gists.

   

    

### SYNTAX

New-Gist [[-InputObject] <PSObject>] [-File <String>] [-Description <String>] [-Username <String>] [-Public] [<Comm

    onParameters>]

    

    

### DESCRIPTION

Publishes files as Owned or Anonymous Github Gists.

    



### PARAMETERS

-InputObject <PSObject>

        Accepts a series of files which will be published as a single Gist

        

-File <String>

        A single file path to be published as a Gist.

        

-Description <String>

        (optional) The Description of this Gist.

        

-Username <String>

        The Github username which will own this Gist.

        

-Public [<SwitchParameter>]

When specified, the Gist will be made public.  Default is private.

        

<CommonParameters>

		This cmdlet supports the common parameters: Verbose, Debug,

		ErrorAction, ErrorVariable, WarningAction, WarningVariable,

		OutBuffer and OutVariable. For more information, type,

		"get-help about_commonparameters".



EXAMPLE 1 - Publishing a public Gist

    

    gist -File "Hello.js" -Description "Hello.js greets all visitors"

    

EXAMPLE 2 - Publishing a private Gist

    

    gist -File "Hello.js" -Description "Hello.js greets all visitors" -Public


EXAMPLE 3 - Publish a directory as gist

    ls | gist -Description "Holy awesome batman!" -Public

