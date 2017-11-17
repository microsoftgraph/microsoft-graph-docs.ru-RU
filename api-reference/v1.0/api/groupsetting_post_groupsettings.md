# <a name="create-a-group-setting"></a><span data-ttu-id="620f3-101">Создание параметра группы</span><span class="sxs-lookup"><span data-stu-id="620f3-101">Create a group setting</span></span>

<span data-ttu-id="620f3-p101">Этот API позволяет создавать новые параметры на базе шаблонов, доступных в объектах [groupSettingTemplate](../resources/groupsettingtemplate.md). Эти параметры можно использовать как на уровне клиента, так и на уровне группы. Запрос на создание должен предоставлять объекты [settingValue](../resources/settingvalue.md) для всех параметров, определенных в шаблоне. Специально для групп можно задавать только параметр, разрешающий или запрещающий членам группы приглашать пользователей-гостей. Возможность добавлять пользователей-гостей в группу общедоступна, поэтому данный параметр позволит контролировать подобное поведение.</span><span class="sxs-lookup"><span data-stu-id="620f3-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

## <a name="permissions"></a><span data-ttu-id="620f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="620f3-107">Permissions</span></span>

<span data-ttu-id="620f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="620f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="620f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="620f3-110">Permission type</span></span>      | <span data-ttu-id="620f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="620f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="620f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="620f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="620f3-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="620f3-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="620f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="620f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="620f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620f3-115">Not supported.</span></span>    |
|<span data-ttu-id="620f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="620f3-116">Application</span></span> | <span data-ttu-id="620f3-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="620f3-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="620f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="620f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="620f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="620f3-119">Request headers</span></span>

| <span data-ttu-id="620f3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="620f3-120">Name</span></span> | <span data-ttu-id="620f3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="620f3-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="620f3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="620f3-122">Authorization</span></span> | <span data-ttu-id="620f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="620f3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="620f3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="620f3-125">Content-Type</span></span> | <span data-ttu-id="620f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="620f3-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="620f3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="620f3-127">Request body</span></span>
<span data-ttu-id="620f3-p104">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.</span><span class="sxs-lookup"><span data-stu-id="620f3-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="620f3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="620f3-130">Response</span></span>

<span data-ttu-id="620f3-131">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="620f3-131">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="620f3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="620f3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="620f3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="620f3-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="620f3-134">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="620f3-134">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="620f3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="620f3-135">Response</span></span>

<span data-ttu-id="620f3-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="620f3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ],
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->