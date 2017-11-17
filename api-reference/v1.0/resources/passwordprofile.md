# <a name="passwordprofile-resource-type"></a><span data-ttu-id="81fc3-101">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="81fc3-101">passwordProfile resource type</span></span>

<span data-ttu-id="81fc3-p101">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="81fc3-p101">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="81fc3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="81fc3-104">Properties</span></span>
| <span data-ttu-id="81fc3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="81fc3-105">Property</span></span>     | <span data-ttu-id="81fc3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="81fc3-106">Type</span></span>   |<span data-ttu-id="81fc3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="81fc3-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81fc3-108">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="81fc3-108">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="81fc3-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="81fc3-109">Boolean</span></span>| <span data-ttu-id="81fc3-110">Значение **true** указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="81fc3-110">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="81fc3-111">password</span><span class="sxs-lookup"><span data-stu-id="81fc3-111">password</span></span>|<span data-ttu-id="81fc3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="81fc3-112">String</span></span>|<span data-ttu-id="81fc3-p102">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="81fc3-p102">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81fc3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81fc3-118">JSON representation</span></span>

<span data-ttu-id="81fc3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81fc3-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->