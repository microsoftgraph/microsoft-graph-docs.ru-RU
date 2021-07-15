---
title: Обновление tenantCustomizedInformation
description: Обновление свойств объекта tenantCustomizedInformation.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 3f43e7e3f543c0a74b27a3594f573d4fe3cc68c6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441860"
---
# <a name="update-tenantcustomizedinformation"></a><span data-ttu-id="c7ee2-103">Обновление tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="c7ee2-103">Update tenantCustomizedInformation</span></span>
<span data-ttu-id="c7ee2-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c7ee2-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ee2-105">Обновление свойств объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-105">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7ee2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ee2-106">Permissions</span></span>
<span data-ttu-id="c7ee2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ee2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ee2-109">Permission type</span></span>|<span data-ttu-id="c7ee2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ee2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ee2-112">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ee2-112">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="c7ee2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ee2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-114">Not supported.</span></span>|
|<span data-ttu-id="c7ee2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7ee2-115">Application</span></span>|<span data-ttu-id="c7ee2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ee2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ee2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="request-headers"></a><span data-ttu-id="c7ee2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7ee2-118">Request headers</span></span>
|<span data-ttu-id="c7ee2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c7ee2-119">Name</span></span>|<span data-ttu-id="c7ee2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ee2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7ee2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7ee2-121">Authorization</span></span>|<span data-ttu-id="c7ee2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7ee2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7ee2-124">Content-Type</span></span>|<span data-ttu-id="c7ee2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ee2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ee2-127">Request body</span></span>
<span data-ttu-id="c7ee2-128">В теле запроса поставляем представление JSON объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-128">In the request body, supply a JSON representation of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

<span data-ttu-id="c7ee2-129">В следующей таблице показаны свойства, необходимые при обновлении [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-129">The following table shows the properties that are required when you update the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span></span>

|<span data-ttu-id="c7ee2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ee2-130">Property</span></span>|<span data-ttu-id="c7ee2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ee2-131">Type</span></span>|<span data-ttu-id="c7ee2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ee2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ee2-133">id</span><span class="sxs-lookup"><span data-stu-id="c7ee2-133">id</span></span>|<span data-ttu-id="c7ee2-134">String</span><span class="sxs-lookup"><span data-stu-id="c7ee2-134">String</span></span>|<span data-ttu-id="c7ee2-135">Идентификатор Azure Active Directory клиента для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-135">The Azure Active Directory tenant identifier for the managed tenant.</span></span>|
|<span data-ttu-id="c7ee2-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="c7ee2-136">tenantId</span></span>|<span data-ttu-id="c7ee2-137">String</span><span class="sxs-lookup"><span data-stu-id="c7ee2-137">String</span></span>|<span data-ttu-id="c7ee2-138">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-138">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="c7ee2-139">contacts</span><span class="sxs-lookup"><span data-stu-id="c7ee2-139">contacts</span></span>|<span data-ttu-id="c7ee2-140">[коллекция microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c7ee2-140">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="c7ee2-141">Коллекция контактов, связанных с управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-141">The collection of contacts associated with the managed tenant.</span></span>|
|<span data-ttu-id="c7ee2-142">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="c7ee2-142">website</span></span>|<span data-ttu-id="c7ee2-143">String</span><span class="sxs-lookup"><span data-stu-id="c7ee2-143">String</span></span>|<span data-ttu-id="c7ee2-144">Веб-сайт управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-144">The website for the managed tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="c7ee2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ee2-145">Response</span></span>

<span data-ttu-id="c7ee2-146">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-146">If successful, this method returns a `200 OK` response code and an updated [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7ee2-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7ee2-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7ee2-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ee2-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7ee2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7ee2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenantcustomizedinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
Content-Type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="c7ee2-150">C#</span><span class="sxs-lookup"><span data-stu-id="c7ee2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenantcustomizedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7ee2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7ee2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenantcustomizedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7ee2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7ee2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenantcustomizedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7ee2-153">Java</span><span class="sxs-lookup"><span data-stu-id="c7ee2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenantcustomizedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c7ee2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ee2-154">Response</span></span>
><span data-ttu-id="c7ee2-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7ee2-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "website": "https://www.fourthcoffee.com",
  "contacts": [
    {
      "name": "Sally",
      "email": "sally@fourthcoffee.com",
      "phone": "5558009731"
    },
    {
      "name": "Hector",
      "email": "hector@fourthcoffee.com",
      "phone": "5558009732"
    }
  ]
}
```
