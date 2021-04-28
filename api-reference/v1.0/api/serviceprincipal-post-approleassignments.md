---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставление назначения роли приложения субъекту-службе
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: e8021b9bcc96e0a70a139e5d4fd1597f186ab20b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054422"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="62a35-103">Предоставление appRoleAssignment субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="62a35-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="62a35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a35-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="62a35-105">Назначьте роль приложения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="62a35-105">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="62a35-106">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="62a35-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="62a35-107">Разрешения приложения можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="62a35-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="62a35-108">Чтобы предоставить назначение роли приложения субъекту-службе клиента, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="62a35-108">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="62a35-109">`principalId`: `id` субъекта-службы клиента, которой нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="62a35-109">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="62a35-110">`resourceId`: `id` ресурса `servicePrincipal` (API), в которых определена роль приложения (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="62a35-110">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="62a35-111">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения субъекту-службе клиента.</span><span class="sxs-lookup"><span data-stu-id="62a35-111">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="62a35-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62a35-112">Permissions</span></span>

<span data-ttu-id="62a35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a35-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62a35-115">Permission type</span></span>      | <span data-ttu-id="62a35-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62a35-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62a35-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62a35-117">Delegated (work or school account)</span></span> | <span data-ttu-id="62a35-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62a35-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62a35-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62a35-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a35-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a35-120">Not supported.</span></span>    |
|<span data-ttu-id="62a35-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62a35-121">Application</span></span> | <span data-ttu-id="62a35-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a35-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62a35-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62a35-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="62a35-124">Рекомендуется создавать назначения ролей приложения, используя [`appRoleAssignedTo`отношение _ресурса_ субъекта-службы](serviceprincipal-post-approleassignedto.md) вместо `appRoleAssignments`отношения назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="62a35-124">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62a35-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62a35-125">Request headers</span></span>

| <span data-ttu-id="62a35-126">Имя</span><span class="sxs-lookup"><span data-stu-id="62a35-126">Name</span></span>       | <span data-ttu-id="62a35-127">Описание</span><span class="sxs-lookup"><span data-stu-id="62a35-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="62a35-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62a35-128">Authorization</span></span> | <span data-ttu-id="62a35-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62a35-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62a35-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62a35-131">Content-type</span></span> | <span data-ttu-id="62a35-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62a35-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62a35-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62a35-134">Request body</span></span>

<span data-ttu-id="62a35-135">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="62a35-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="62a35-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="62a35-136">Response</span></span>

<span data-ttu-id="62a35-137">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="62a35-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62a35-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="62a35-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62a35-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="62a35-139">Request</span></span>

<span data-ttu-id="62a35-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62a35-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62a35-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="62a35-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments
Content-Type: application/json

{
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}
```
# <a name="c"></a>[<span data-ttu-id="62a35-142">C#</span><span class="sxs-lookup"><span data-stu-id="62a35-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62a35-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62a35-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62a35-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62a35-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62a35-145">Java</span><span class="sxs-lookup"><span data-stu-id="62a35-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="62a35-p105">В этом примере обратите внимание, что значение, используемое в качестве **ИД** субъекта службы в URL-адресе запроса (`9028d19c-26a9-4809-8e3f-20ff73e2d75e`), совпадает со свойством **principalId** в тексте. Значение **resourceId** является **ИД** для субъекта-службы ресурса (API).</span><span class="sxs-lookup"><span data-stu-id="62a35-p105">In this example, note that the value used as the service principal **id** in the request URL (`9028d19c-26a9-4809-8e3f-20ff73e2d75e`) is the same as the **principalId** property in the body. The **resourceId** value is the **id** of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="62a35-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="62a35-148">Response</span></span>

<span data-ttu-id="62a35-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62a35-149">Here is an example of the response.</span></span> 

> <span data-ttu-id="62a35-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62a35-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments/$entity",
  "id": "2jLOj0YSe0OZzXbR1Gd71fDqFUrPM1xIgUfvWBHJ9n0",
  "createdDateTime": "2021-02-15T16:39:38.2975029Z",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6",
  "principalDisplayName": "Fabrikam App",
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "principalType": "ServicePrincipal",
  "resourceDisplayName": "Microsoft Graph",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
