# CNN-Classification-Model-for-Molecule-class-prediction

* ### Data Info:

  * molecule_name: Symbolic name of each molecule. Musks have names such as MUSK-188. Non-musks have names such as NON-MUSK-jp13.

  * conformation_name: Symbolic name of each conformation. These have the format MOL_ISO+CONF, where MOL is the molecule number, ISO is the stereoisomer number (usually 1), and CONF is the conformation number.

  * f1 through f162: These are "distance features" along rays (see paper cited above). The distances are measured in hundredths of Angstroms. The distances may be negative or positive, since they are actually measured relative to an origin placed along each ray. The origin was defined by a "consensus musk" surface that is no longer used. Hence, any experiments with the data should treat these feature values as lying on an arbitrary continuous scale. In particular, the algorithm should not make any use of the zero point or the sign of each feature value.

  * f163: This is the distance of the oxygen atom in the molecule to a designated point in 3-space. This is also called OXY-DIS.

  * f164: OXY-X: X-displacement from the designated point.

  * f165: OXY-Y: Y-displacement from the designated point.

  * f166: OXY-Z: Z-displacement from the designated point.

  * class: 0 => non-musk, 1 => musk
