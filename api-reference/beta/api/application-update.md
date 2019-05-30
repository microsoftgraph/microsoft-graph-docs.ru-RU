---
title: Обновление приложения
description: Обновление свойств объекта Application.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2984e7d57144fd6d5e3efee7d6c9a9c8d68c529c
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34535996"
---
# <a name="update-application"></a><span data-ttu-id="fa568-103">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="fa568-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa568-104">Обновление свойств объекта Application.</span><span class="sxs-lookup"><span data-stu-id="fa568-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa568-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa568-105">Permissions</span></span>
<span data-ttu-id="fa568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa568-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa568-108">Permission type</span></span>      | <span data-ttu-id="fa568-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa568-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa568-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa568-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa568-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa568-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa568-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa568-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa568-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa568-113">Not supported.</span></span>    |
|<span data-ttu-id="fa568-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa568-114">Application</span></span> | <span data-ttu-id="fa568-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa568-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa568-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa568-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fa568-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa568-117">Request headers</span></span>
| <span data-ttu-id="fa568-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fa568-118">Name</span></span>       | <span data-ttu-id="fa568-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fa568-119">Type</span></span> | <span data-ttu-id="fa568-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa568-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa568-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa568-121">Authorization</span></span>  | <span data-ttu-id="fa568-122">string</span><span class="sxs-lookup"><span data-stu-id="fa568-122">string</span></span>  | <span data-ttu-id="fa568-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa568-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa568-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa568-125">Request body</span></span>
<span data-ttu-id="fa568-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fa568-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa568-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa568-129">Property</span></span>     | <span data-ttu-id="fa568-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fa568-130">Type</span></span>   |<span data-ttu-id="fa568-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fa568-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa568-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="fa568-132">allowPublicClient</span></span>|<span data-ttu-id="fa568-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa568-133">Boolean</span></span>| <span data-ttu-id="fa568-134">Указывает, может ли приложение работать в качестве общедоступного клиента.</span><span class="sxs-lookup"><span data-stu-id="fa568-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="fa568-135">Например, установленное приложение, запущенное на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa568-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="fa568-136">Значение по умолчанию: *false*.</span><span class="sxs-lookup"><span data-stu-id="fa568-136">Default value is *false*.</span></span> |
|<span data-ttu-id="fa568-137">api</span><span class="sxs-lookup"><span data-stu-id="fa568-137">api</span></span>|[<span data-ttu-id="fa568-138">apiApplication</span><span class="sxs-lookup"><span data-stu-id="fa568-138">apiApplication</span></span>](../resources/apiapplication.md)| <span data-ttu-id="fa568-139">Указывает параметры для приложения API.</span><span class="sxs-lookup"><span data-stu-id="fa568-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="fa568-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="fa568-140">appRoles</span></span>|<span data-ttu-id="fa568-141">Коллекция [appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="fa568-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="fa568-142">Коллекция ролей приложения, которые могут быть объявлены приложением.</span><span class="sxs-lookup"><span data-stu-id="fa568-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="fa568-143">Эти роли могут назначаться пользователям, группам или субъектам-службам.</span><span class="sxs-lookup"><span data-stu-id="fa568-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="fa568-144">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-144">Not nullable.</span></span>|
|<span data-ttu-id="fa568-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="fa568-145">applicationAliases</span></span>|<span data-ttu-id="fa568-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa568-146">String collection</span></span>| <span data-ttu-id="fa568-147">URI, определяющие приложение.</span><span class="sxs-lookup"><span data-stu-id="fa568-147">The URIs that identify the application.</span></span> <span data-ttu-id="fa568-148">Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span><span class="sxs-lookup"><span data-stu-id="fa568-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="fa568-149">Для выражений фильтра в случае многозначных свойств требуется оператор *any*.</span><span class="sxs-lookup"><span data-stu-id="fa568-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="fa568-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-150">Not nullable.</span></span> |
|<span data-ttu-id="fa568-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa568-151">createdDateTime</span></span>|<span data-ttu-id="fa568-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa568-152">DateTimeOffset</span></span>| <span data-ttu-id="fa568-153">Дата и время регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="fa568-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa568-154">deletedDateTime</span></span>|<span data-ttu-id="fa568-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa568-155">DateTimeOffset</span></span>| <span data-ttu-id="fa568-156">Дата и время удаления приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="fa568-157">displayName</span><span class="sxs-lookup"><span data-stu-id="fa568-157">displayName</span></span>|<span data-ttu-id="fa568-158">Строка</span><span class="sxs-lookup"><span data-stu-id="fa568-158">String</span></span>|<span data-ttu-id="fa568-159">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-159">The display name for the application.</span></span> |
|<span data-ttu-id="fa568-160">id</span><span class="sxs-lookup"><span data-stu-id="fa568-160">id</span></span>|<span data-ttu-id="fa568-161">String</span><span class="sxs-lookup"><span data-stu-id="fa568-161">String</span></span>|<span data-ttu-id="fa568-162">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-162">The unique identifier for the application.</span></span> <span data-ttu-id="fa568-163">Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="fa568-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="fa568-164">Ключ.</span><span class="sxs-lookup"><span data-stu-id="fa568-164">Key.</span></span> <span data-ttu-id="fa568-165">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-165">Not nullable.</span></span> <span data-ttu-id="fa568-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa568-166">Read-only.</span></span> |
|<span data-ttu-id="fa568-167">info</span><span class="sxs-lookup"><span data-stu-id="fa568-167">info</span></span>|[<span data-ttu-id="fa568-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="fa568-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="fa568-169">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-169">Basic profile information of the application.</span></span> | <span data-ttu-id="fa568-170">Указывает параметры для установленных клиентов, например классических или мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="fa568-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="fa568-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="fa568-171">keyCredentials</span></span>|<span data-ttu-id="fa568-172">Коллекция [keyCredential](../resources/keycredential.md)</span><span class="sxs-lookup"><span data-stu-id="fa568-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="fa568-173">Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="fa568-174">logo</span><span class="sxs-lookup"><span data-stu-id="fa568-174">logo</span></span>|<span data-ttu-id="fa568-175">Stream</span><span class="sxs-lookup"><span data-stu-id="fa568-175">Stream</span></span>|<span data-ttu-id="fa568-176">Основной логотип для приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-176">The main logo for the application.</span></span> <span data-ttu-id="fa568-177">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-177">Not nullable.</span></span> |
|<span data-ttu-id="fa568-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="fa568-178">orgRestrictions</span></span>|<span data-ttu-id="fa568-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa568-179">String collection</span></span>| <span data-ttu-id="fa568-180">Организационное Тенантидс, к которому приложение ограничено.</span><span class="sxs-lookup"><span data-stu-id="fa568-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="fa568-181">Если коллекция пуста, приложение является несколькими клиентами (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="fa568-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="fa568-182">Если коллекция содержит Тенантидс, приложение ограничено Тенантидс Организации в коллекции.</span><span class="sxs-lookup"><span data-stu-id="fa568-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="fa568-183">Указание других клиентов, кроме tenantId, где зарегистрировано приложение, предполагает косвенное включение собственного tenantId приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="fa568-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="fa568-184">passwordCredentials</span></span>|<span data-ttu-id="fa568-185">Коллекция [passwordCredential](../resources/passwordcredential.md)</span><span class="sxs-lookup"><span data-stu-id="fa568-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="fa568-186">Коллекция учетных данных паролей, связанных с приложением.</span><span class="sxs-lookup"><span data-stu-id="fa568-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="fa568-187">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-187">Not nullable.</span></span>|
|<span data-ttu-id="fa568-188">Преаусоризедаппликатионс</span><span class="sxs-lookup"><span data-stu-id="fa568-188">preAuthorizedApplications</span></span>|<span data-ttu-id="fa568-189">Коллекция [preAuthorizedApplication](../resources/preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="fa568-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="fa568-190">Перечисляет приложения и запрашиваемые разрешения для неявного согласия.</span><span class="sxs-lookup"><span data-stu-id="fa568-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="fa568-191">Необходимо, чтобы администратор предоставил согласие на применение приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="fa568-192">Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="fa568-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="fa568-193">Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa568-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="fa568-194">Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa568-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="fa568-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="fa568-195">requiredResourceAccess</span></span>|<span data-ttu-id="fa568-196">Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="fa568-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="fa568-197">Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fa568-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="fa568-198">Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия.</span><span class="sxs-lookup"><span data-stu-id="fa568-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="fa568-199">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fa568-199">Not nullable.</span></span>|
|<span data-ttu-id="fa568-200">tags</span><span class="sxs-lookup"><span data-stu-id="fa568-200">tags</span></span>|<span data-ttu-id="fa568-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa568-201">String collection</span></span>| <span data-ttu-id="fa568-202">Настраиваемые строки, которые можно использовать для классификации и определения приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="fa568-203">web</span><span class="sxs-lookup"><span data-stu-id="fa568-203">web</span></span>|[<span data-ttu-id="fa568-204">webApplication</span><span class="sxs-lookup"><span data-stu-id="fa568-204">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="fa568-205">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="fa568-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="fa568-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa568-206">Response</span></span>

<span data-ttu-id="fa568-207">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa568-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa568-208">Пример</span><span class="sxs-lookup"><span data-stu-id="fa568-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa568-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa568-209">Request</span></span>
<span data-ttu-id="fa568-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa568-210">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a><span data-ttu-id="fa568-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa568-211">Response</span></span>
<span data-ttu-id="fa568-212">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fa568-212">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa568-213">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fa568-213">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fa568-214">C#</span><span class="sxs-lookup"><span data-stu-id="fa568-214">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa568-215">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa568-215">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_application-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
