---
title: 'cloudPcUserSetting: назначение'
description: Назначение параметров пользователя облачного КОМПЬЮТЕРА группам пользователей.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 5279a630f3ba9eeb684a98552e8f0184ab441098
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207118"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="127ba-103">cloudPcUserSetting: назначение</span><span class="sxs-lookup"><span data-stu-id="127ba-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="127ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="127ba-105">Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="127ba-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="127ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="127ba-106">Permissions</span></span>

<span data-ttu-id="127ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="127ba-109">Permission type</span></span>|<span data-ttu-id="127ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="127ba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="127ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="127ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="127ba-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127ba-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="127ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="127ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="127ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="127ba-114">Not supported.</span></span>|
|<span data-ttu-id="127ba-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="127ba-115">Application</span></span>|<span data-ttu-id="127ba-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127ba-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="127ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="127ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="127ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="127ba-118">Request headers</span></span>

|<span data-ttu-id="127ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="127ba-119">Name</span></span>|<span data-ttu-id="127ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="127ba-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="127ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="127ba-121">Authorization</span></span>|<span data-ttu-id="127ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="127ba-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="127ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="127ba-124">Content-Type</span></span>|<span data-ttu-id="127ba-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="127ba-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="127ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="127ba-127">Request body</span></span>

<span data-ttu-id="127ba-128">В корпусе запроса поставляем представление JSON объекта [cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="127ba-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

|<span data-ttu-id="127ba-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="127ba-129">Parameter</span></span>|<span data-ttu-id="127ba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="127ba-130">Type</span></span>|<span data-ttu-id="127ba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="127ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127ba-132">assignments</span><span class="sxs-lookup"><span data-stu-id="127ba-132">assignments</span></span>|<span data-ttu-id="127ba-133">[коллекция cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="127ba-133">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span> | <span data-ttu-id="127ba-134">Коллекция пользовательских облачных КОМПЬЮТЕРов, устанавливая ресурсы, которые должны быть назначены соответствующей целевой группе.</span><span class="sxs-lookup"><span data-stu-id="127ba-134">The collection of cloud PC user setting resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="127ba-135">В Microsoft 365 поддерживаются только группы и группы безопасности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="127ba-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="127ba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="127ba-136">Response</span></span>

<span data-ttu-id="127ba-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="127ba-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="127ba-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="127ba-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="127ba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="127ba-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="127ba-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="127ba-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="127ba-141">C#</span><span class="sxs-lookup"><span data-stu-id="127ba-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcusersetting-assign-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="127ba-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="127ba-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcusersetting-assign-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="127ba-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="127ba-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcusersetting-assign-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="127ba-144">Java</span><span class="sxs-lookup"><span data-stu-id="127ba-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcusersetting-assign-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="127ba-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="127ba-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
