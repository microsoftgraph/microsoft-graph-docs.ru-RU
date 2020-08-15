---
title: Обновление Акцесспаккаже
description: Обновление свойств объекта Акцесспаккаже.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 919a9f6a87463313d0193f3d8d43234654f3952f
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757486"
---
# <a name="update-accesspackage"></a><span data-ttu-id="70d94-103">Обновление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="70d94-103">Update accessPackage</span></span>

<span data-ttu-id="70d94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70d94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70d94-105">Обновление существующего объекта [акцесспаккаже](../resources/accesspackage.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="70d94-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="70d94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70d94-106">Permissions</span></span>
<span data-ttu-id="70d94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="70d94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="70d94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70d94-109">Permission type</span></span>|<span data-ttu-id="70d94-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70d94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70d94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70d94-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70d94-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d94-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="70d94-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70d94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70d94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70d94-114">Not supported.</span></span> |
|<span data-ttu-id="70d94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70d94-115">Application</span></span>                            | <span data-ttu-id="70d94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70d94-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70d94-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70d94-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="70d94-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70d94-118">Request headers</span></span>
|<span data-ttu-id="70d94-119">Имя</span><span class="sxs-lookup"><span data-stu-id="70d94-119">Name</span></span>|<span data-ttu-id="70d94-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70d94-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70d94-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70d94-121">Authorization</span></span>|<span data-ttu-id="70d94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70d94-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="70d94-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70d94-124">Content-Type</span></span>|<span data-ttu-id="70d94-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70d94-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70d94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70d94-127">Request body</span></span>
<span data-ttu-id="70d94-128">В тексте запроса добавьте представление параметров объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70d94-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="70d94-129">В следующей таблице приведены свойства, которые можно указать при обновлении [акцесспаккаже](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="70d94-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="70d94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="70d94-130">Property</span></span>|<span data-ttu-id="70d94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="70d94-131">Type</span></span>|<span data-ttu-id="70d94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="70d94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70d94-133">displayName</span><span class="sxs-lookup"><span data-stu-id="70d94-133">displayName</span></span>|<span data-ttu-id="70d94-134">Строка</span><span class="sxs-lookup"><span data-stu-id="70d94-134">String</span></span>|<span data-ttu-id="70d94-135">Имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="70d94-135">The access package name.</span></span>|
|<span data-ttu-id="70d94-136">description</span><span class="sxs-lookup"><span data-stu-id="70d94-136">description</span></span>|<span data-ttu-id="70d94-137">String</span><span class="sxs-lookup"><span data-stu-id="70d94-137">String</span></span>|<span data-ttu-id="70d94-138">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="70d94-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="70d94-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="70d94-139">Response</span></span>
<span data-ttu-id="70d94-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70d94-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="70d94-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="70d94-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70d94-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="70d94-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json
Content-length: 38

{
  "displayName":"Access Package New Name"
}
```


### <a name="response"></a><span data-ttu-id="70d94-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="70d94-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
