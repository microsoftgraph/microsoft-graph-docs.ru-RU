---
title: Создание Коннектедорганизатион
description: Создание нового Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 47e8ba9564b1810da99e212ab9832142656d18f0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510237"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="ea102-103">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="ea102-103">Create connectedOrganization</span></span>

<span data-ttu-id="ea102-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea102-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea102-105">Создание нового объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="ea102-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea102-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea102-106">Permissions</span></span>

<span data-ttu-id="ea102-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea102-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea102-109">Permission type</span></span>|<span data-ttu-id="ea102-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea102-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="ea102-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea102-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea102-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea102-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ea102-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea102-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea102-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea102-114">Not supported.</span></span> |
| <span data-ttu-id="ea102-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea102-115">Application</span></span>                            | <span data-ttu-id="ea102-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea102-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea102-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea102-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="ea102-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea102-118">Request headers</span></span>

|<span data-ttu-id="ea102-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ea102-119">Name</span></span>|<span data-ttu-id="ea102-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ea102-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ea102-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea102-121">Authorization</span></span>|<span data-ttu-id="ea102-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea102-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ea102-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea102-124">Content-Type</span></span>|<span data-ttu-id="ea102-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea102-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea102-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea102-127">Request body</span></span>
<span data-ttu-id="ea102-128">В тексте запроса добавьте представление объекта [коннектедорганизатион](../resources/connectedorganization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea102-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="ea102-129">В следующей таблице приведены свойства, необходимые при создании [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="ea102-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="ea102-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea102-130">Property</span></span>|<span data-ttu-id="ea102-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea102-131">Type</span></span>|<span data-ttu-id="ea102-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea102-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea102-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ea102-133">displayName</span></span>|<span data-ttu-id="ea102-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ea102-134">String</span></span>|<span data-ttu-id="ea102-135">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="ea102-135">The connected organization name.</span></span> |
|<span data-ttu-id="ea102-136">description</span><span class="sxs-lookup"><span data-stu-id="ea102-136">description</span></span>|<span data-ttu-id="ea102-137">String</span><span class="sxs-lookup"><span data-stu-id="ea102-137">String</span></span>|<span data-ttu-id="ea102-138">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="ea102-138">The connected organization description.</span></span>|
|<span data-ttu-id="ea102-139">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="ea102-139">identitySources</span></span>|<span data-ttu-id="ea102-140">Коллекция [идентитисаурце](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="ea102-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="ea102-141">Коллекция с одним элементом — начальным источником идентификаторов в этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="ea102-141">A collection with one element, the initial identity source in this connected organization.</span></span>|


## <a name="response"></a><span data-ttu-id="ea102-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea102-142">Response</span></span>

<span data-ttu-id="ea102-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea102-143">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea102-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea102-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea102-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea102-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ea102-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea102-146">Response</span></span>
<span data-ttu-id="ea102-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea102-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-06-08T20:13:53.7099947Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
