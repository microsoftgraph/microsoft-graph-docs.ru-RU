---
title: Создание параметра группы
description: Создайте новый параметр на основе шаблонов, доступных в groupSettingTemplates.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2d85876b4dc024f976e6bedbc7aadd17eda5cec7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054009"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="37ab2-103">Создание параметра группы</span><span class="sxs-lookup"><span data-stu-id="37ab2-103">Create a group setting</span></span>

<span data-ttu-id="37ab2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37ab2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37ab2-105">Используйте этот API для создания нового параметра на основе шаблонов, доступных в [groupSettingTemplates.](../resources/groupsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="37ab2-105">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md).</span></span> <span data-ttu-id="37ab2-106">Эти параметры могут быть на уровне клиента или на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="37ab2-106">These settings can be at the tenant-level or at the group level.</span></span> <span data-ttu-id="37ab2-107">Запрос на создание должен предоставить [параметрValues](../resources/settingvalue.md) для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="37ab2-107">The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template.</span></span> <span data-ttu-id="37ab2-108">Для параметров, определенных для группы, можно установить только параметр, регуляющий, могут ли члены группы приглашать гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="37ab2-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="37ab2-109">Это будет регулировать такое поведение после того, как будет доступна возможность добавлять гостевых пользователей в группу.</span><span class="sxs-lookup"><span data-stu-id="37ab2-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span> <span data-ttu-id="37ab2-110">Для конечных точек бета-версии используйте [directorySettingTemplates.](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="37ab2-110">For beta endpoints, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta).</span></span>

## <a name="permissions"></a><span data-ttu-id="37ab2-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37ab2-111">Permissions</span></span>

<span data-ttu-id="37ab2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37ab2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37ab2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37ab2-114">Permission type</span></span>      | <span data-ttu-id="37ab2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37ab2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37ab2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37ab2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="37ab2-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37ab2-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37ab2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37ab2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37ab2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37ab2-119">Not supported.</span></span>    |
|<span data-ttu-id="37ab2-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="37ab2-120">Application</span></span> | <span data-ttu-id="37ab2-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ab2-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37ab2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37ab2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="37ab2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37ab2-123">Request headers</span></span>

| <span data-ttu-id="37ab2-124">Имя</span><span class="sxs-lookup"><span data-stu-id="37ab2-124">Name</span></span> | <span data-ttu-id="37ab2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="37ab2-125">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="37ab2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37ab2-126">Authorization</span></span> | <span data-ttu-id="37ab2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37ab2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37ab2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37ab2-129">Content-Type</span></span> | <span data-ttu-id="37ab2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="37ab2-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="37ab2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37ab2-131">Request body</span></span>
<span data-ttu-id="37ab2-p104">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.</span><span class="sxs-lookup"><span data-stu-id="37ab2-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="37ab2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37ab2-134">Response</span></span>

<span data-ttu-id="37ab2-135">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37ab2-135">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ab2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="37ab2-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="37ab2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="37ab2-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37ab2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="37ab2-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37ab2-139">C#</span><span class="sxs-lookup"><span data-stu-id="37ab2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37ab2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37ab2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37ab2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37ab2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37ab2-142">Java</span><span class="sxs-lookup"><span data-stu-id="37ab2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="37ab2-143">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37ab2-143">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="37ab2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="37ab2-144">Response</span></span>

<span data-ttu-id="37ab2-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37ab2-145">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

