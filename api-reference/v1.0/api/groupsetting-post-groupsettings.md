---
title: Создание параметра группы
description: Создайте новый параметр на основе шаблонов, доступных в Граупсеттингтемплатес.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b96a198543da31e9abb672801e56a8ab1d92e0d5
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373995"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="e07d0-103">Создание параметра группы</span><span class="sxs-lookup"><span data-stu-id="e07d0-103">Create a group setting</span></span>

<span data-ttu-id="e07d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e07d0-105">Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в [граупсеттингтемплатес](../resources/groupsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e07d0-105">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md).</span></span> <span data-ttu-id="e07d0-106">Эти параметры могут быть на уровне клиента или на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="e07d0-106">These settings can be at the tenant-level or at the group level.</span></span> <span data-ttu-id="e07d0-107">Запрос на создание должен предоставлять [сеттингвалуес](../resources/settingvalue.md) для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="e07d0-107">The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template.</span></span> <span data-ttu-id="e07d0-108">Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="e07d0-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="e07d0-109">Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.</span><span class="sxs-lookup"><span data-stu-id="e07d0-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span> <span data-ttu-id="e07d0-110">Для конечных точек бета-версии используйте [директорисеттингтемплатес](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e07d0-110">For beta endpoints, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta).</span></span>

## <a name="permissions"></a><span data-ttu-id="e07d0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e07d0-111">Permissions</span></span>

<span data-ttu-id="e07d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e07d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e07d0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e07d0-114">Permission type</span></span>      | <span data-ttu-id="e07d0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e07d0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e07d0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e07d0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e07d0-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e07d0-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e07d0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e07d0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e07d0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e07d0-119">Not supported.</span></span>    |
|<span data-ttu-id="e07d0-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="e07d0-120">Application</span></span> | <span data-ttu-id="e07d0-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07d0-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e07d0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e07d0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="e07d0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e07d0-123">Request headers</span></span>

| <span data-ttu-id="e07d0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e07d0-124">Name</span></span> | <span data-ttu-id="e07d0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e07d0-125">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e07d0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e07d0-126">Authorization</span></span> | <span data-ttu-id="e07d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e07d0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e07d0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e07d0-129">Content-Type</span></span> | <span data-ttu-id="e07d0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e07d0-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e07d0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e07d0-131">Request body</span></span>
<span data-ttu-id="e07d0-p104">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.</span><span class="sxs-lookup"><span data-stu-id="e07d0-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="e07d0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e07d0-134">Response</span></span>

<span data-ttu-id="e07d0-135">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e07d0-135">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e07d0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e07d0-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e07d0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e07d0-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e07d0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e07d0-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e07d0-139">C#</span><span class="sxs-lookup"><span data-stu-id="e07d0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e07d0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e07d0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e07d0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e07d0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e07d0-142">Java</span><span class="sxs-lookup"><span data-stu-id="e07d0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e07d0-143">В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e07d0-143">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e07d0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e07d0-144">Response</span></span>

<span data-ttu-id="e07d0-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e07d0-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

