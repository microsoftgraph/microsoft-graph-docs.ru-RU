---
title: Создание параметра группы
description: Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Граупсеттингтемплатес. Эти параметры могут быть на уровне клиента или на уровне группы. Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне. Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей. Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8c559455c1525727a9fb397e4578839c8b6356f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613178"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="b5194-107">Создание параметра группы</span><span class="sxs-lookup"><span data-stu-id="b5194-107">Create a group setting</span></span>

<span data-ttu-id="b5194-p102">Этот API позволяет создавать новые параметры на базе шаблонов, доступных в объектах [groupSettingTemplate](../resources/groupsettingtemplate.md). Эти параметры можно использовать как на уровне клиента, так и на уровне группы. Запрос на создание должен предоставлять объекты [settingValue](../resources/settingvalue.md) для всех параметров, определенных в шаблоне. Специально для групп можно задавать только параметр, разрешающий или запрещающий членам группы приглашать пользователей-гостей. Возможность добавлять пользователей-гостей в группу общедоступна, поэтому данный параметр позволит контролировать подобное поведение.</span><span class="sxs-lookup"><span data-stu-id="b5194-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="b5194-113">Чтобы получить список шаблонов и свойств, которые они поддерживают в версии 1.0, используйте [запрос groupSettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0) (для конечных точек бета-версии, вызовите [директорисеттингтемплатес](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span><span class="sxs-lookup"><span data-stu-id="b5194-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="b5194-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5194-114">Permissions</span></span>

<span data-ttu-id="b5194-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5194-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5194-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5194-117">Permission type</span></span>      | <span data-ttu-id="b5194-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5194-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5194-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5194-119">Delegated (work or school account)</span></span> | <span data-ttu-id="b5194-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5194-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5194-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5194-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5194-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5194-122">Not supported.</span></span>    |
|<span data-ttu-id="b5194-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5194-123">Application</span></span> | <span data-ttu-id="b5194-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5194-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5194-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5194-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="b5194-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5194-126">Request headers</span></span>

| <span data-ttu-id="b5194-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b5194-127">Name</span></span> | <span data-ttu-id="b5194-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5194-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b5194-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5194-129">Authorization</span></span> | <span data-ttu-id="b5194-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5194-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5194-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5194-132">Content-Type</span></span> | <span data-ttu-id="b5194-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b5194-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5194-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5194-134">Request body</span></span>
<span data-ttu-id="b5194-p105">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.</span><span class="sxs-lookup"><span data-stu-id="b5194-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="b5194-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5194-137">Response</span></span>

<span data-ttu-id="b5194-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5194-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5194-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b5194-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5194-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5194-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
<span data-ttu-id="b5194-141">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5194-141">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b5194-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5194-142">Response</span></span>

<span data-ttu-id="b5194-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5194-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5194-145">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b5194-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5194-146">Языках</span><span class="sxs-lookup"><span data-stu-id="b5194-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5194-147">Язык</span><span class="sxs-lookup"><span data-stu-id="b5194-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
