# Cloudformation
<br><br>
<p>CloudFormation is an infrastructure automation platform for AWS that deploys AWS resources in a repeatable, testable and auditable manner.</p>
<br>

## Templates
<br> 
<ul>
<li>Text file - YAML or JSON</li>
<li>Cloudformation read template as input</li>
<li>Describe state of the infra</li>
</ul>
<br>

## Stack
<br>
<ul>
<li>Cloudformation reads template and create stack</li>
<li>We update template and update stack to make changes</li>
<li>Set of resources as a single unit.</li>
</ul>
<br>

## Change Set
<br>
<ul>
<li>Before updating a stack, you can generate a change set.</li>
<li>A change set allows you to see how changes will impact your existing resources.</li>
<li>Very important for live systems</li>
</ul>
<br>

## Intrinsic Function
<br>
<p>AWS CloudFormation provides several built-in functions that help you manage your stacks. Use intrinsic functions in your templates to assign values to properties that are not available until runtime.</p>
<br>

## Pseudo Parameters
<br>
<p>Pseudo parameters are parameters that are predefined by AWS CloudFormation. You don't declare them in your template. Use them the same way as you would a parameter, as the argument for the Ref function.</p>
<br>

## Mappings
<br>
<p>The optional Mappings section matches a key to a corresponding set of named values. For example, if you want to set values based on a region, you can create a mapping that uses the region name as a key and contains the values you want to specify for each specific region. You use the Fn::FindInMap intrinsic function to retrieve values in a map.</p>
<br>

## Parameters
<br>
<p>Parameters enable you to input custom values to your template each time you create or update a stack. Use the optional Parameters section to customise your templates. Parameters enable you to input custom values to your template each time you create or update a stack.</p>
<br>

## Outputs
<br>
<p>The optional Outputs section declares output values that you can import into other stacks (to create cross-stack references), return in response (to describe stack calls), or view on the AWS CloudFormation console. For example, you can output the S3 bucket name for a stack to make the bucket easier to find.
</p>
<br>

## Metadata
<br>
<p>Metadata key defines configuration tasks for the cfn-init helper script. This script is useful for configuring and installing applications on EC2 instances. For more information, see AWS::CloudFormation::Init .
</p>