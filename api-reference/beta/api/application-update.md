---
title: Обновление приложения
description: Обновление свойств объекта Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 18b07675304b901bb6b4a37b91c8b48ac0a4ab5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945433"
---
# <a name="update-application"></a><span data-ttu-id="a1352-103">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="a1352-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1352-104">Обновление свойств объекта Application.</span><span class="sxs-lookup"><span data-stu-id="a1352-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1352-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1352-105">Permissions</span></span>
<span data-ttu-id="a1352-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a1352-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1352-108">Permission type</span></span>      | <span data-ttu-id="a1352-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1352-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1352-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1352-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1352-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1352-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1352-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1352-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1352-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1352-113">Not supported.</span></span>    |
|<span data-ttu-id="a1352-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1352-114">Application</span></span> | <span data-ttu-id="a1352-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1352-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1352-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1352-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a1352-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1352-117">Request headers</span></span>
| <span data-ttu-id="a1352-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a1352-118">Name</span></span>       | <span data-ttu-id="a1352-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a1352-119">Type</span></span> | <span data-ttu-id="a1352-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a1352-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1352-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1352-121">Authorization</span></span>  | <span data-ttu-id="a1352-122">string</span><span class="sxs-lookup"><span data-stu-id="a1352-122">string</span></span>  | <span data-ttu-id="a1352-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1352-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1352-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1352-125">Request body</span></span>
<span data-ttu-id="a1352-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a1352-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a1352-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1352-129">Property</span></span>     | <span data-ttu-id="a1352-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1352-130">Type</span></span>   |<span data-ttu-id="a1352-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1352-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1352-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="a1352-132">allowPublicClient</span></span>|<span data-ttu-id="a1352-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1352-133">Boolean</span></span>| <span data-ttu-id="a1352-134">Указывает, может ли приложение работать в качестве общедоступного клиента.</span><span class="sxs-lookup"><span data-stu-id="a1352-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="a1352-135">Например, установленное приложение, запущенное на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a1352-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="a1352-136">Значение по умолчанию: *false*.</span><span class="sxs-lookup"><span data-stu-id="a1352-136">Default value is *false*.</span></span> |
|<span data-ttu-id="a1352-137">api</span><span class="sxs-lookup"><span data-stu-id="a1352-137">api</span></span>|[<span data-ttu-id="a1352-138">apiApplication</span><span class="sxs-lookup"><span data-stu-id="a1352-138">apiApplication</span></span>](../resources/apiapplication.md)| <span data-ttu-id="a1352-139">Указывает параметры для приложения API.</span><span class="sxs-lookup"><span data-stu-id="a1352-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="a1352-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="a1352-140">appRoles</span></span>|<span data-ttu-id="a1352-141">Коллекция [appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="a1352-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="a1352-142">Коллекция ролей приложения, которые могут быть объявлены приложением.</span><span class="sxs-lookup"><span data-stu-id="a1352-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="a1352-143">Эти роли могут назначаться пользователям, группам или субъектам-службам.</span><span class="sxs-lookup"><span data-stu-id="a1352-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="a1352-144">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-144">Not nullable.</span></span>|
|<span data-ttu-id="a1352-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="a1352-145">applicationAliases</span></span>|<span data-ttu-id="a1352-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a1352-146">String collection</span></span>| <span data-ttu-id="a1352-147">URI, определяющие приложение.</span><span class="sxs-lookup"><span data-stu-id="a1352-147">The URIs that identify the application.</span></span> <span data-ttu-id="a1352-148">Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span><span class="sxs-lookup"><span data-stu-id="a1352-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="a1352-149">Для выражений фильтра в случае многозначных свойств требуется оператор *any*.</span><span class="sxs-lookup"><span data-stu-id="a1352-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="a1352-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-150">Not nullable.</span></span> |
|<span data-ttu-id="a1352-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1352-151">createdDateTime</span></span>|<span data-ttu-id="a1352-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1352-152">DateTimeOffset</span></span>| <span data-ttu-id="a1352-153">Дата и время регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="a1352-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1352-154">deletedDateTime</span></span>|<span data-ttu-id="a1352-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1352-155">DateTimeOffset</span></span>| <span data-ttu-id="a1352-156">Дата и время удаления приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="a1352-157">displayName</span><span class="sxs-lookup"><span data-stu-id="a1352-157">displayName</span></span>|<span data-ttu-id="a1352-158">Строка</span><span class="sxs-lookup"><span data-stu-id="a1352-158">String</span></span>|<span data-ttu-id="a1352-159">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-159">The display name for the application.</span></span> |
|<span data-ttu-id="a1352-160">id</span><span class="sxs-lookup"><span data-stu-id="a1352-160">id</span></span>|<span data-ttu-id="a1352-161">String</span><span class="sxs-lookup"><span data-stu-id="a1352-161">String</span></span>|<span data-ttu-id="a1352-162">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-162">The unique identifier for the application.</span></span> <span data-ttu-id="a1352-163">Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a1352-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="a1352-164">Ключ.</span><span class="sxs-lookup"><span data-stu-id="a1352-164">Key.</span></span> <span data-ttu-id="a1352-165">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-165">Not nullable.</span></span> <span data-ttu-id="a1352-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1352-166">Read-only.</span></span> |
|<span data-ttu-id="a1352-167">info</span><span class="sxs-lookup"><span data-stu-id="a1352-167">info</span></span>|[<span data-ttu-id="a1352-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="a1352-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="a1352-169">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-169">Basic profile information of the application.</span></span> | <span data-ttu-id="a1352-170">Указывает параметры для установленных клиентов, например классических или мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="a1352-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="a1352-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="a1352-171">keyCredentials</span></span>|<span data-ttu-id="a1352-172">Коллекция [keyCredential](../resources/keycredential.md)</span><span class="sxs-lookup"><span data-stu-id="a1352-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="a1352-173">Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="a1352-174">logo</span><span class="sxs-lookup"><span data-stu-id="a1352-174">logo</span></span>|<span data-ttu-id="a1352-175">Stream</span><span class="sxs-lookup"><span data-stu-id="a1352-175">Stream</span></span>|<span data-ttu-id="a1352-176">Основной логотип для приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-176">The main logo for the application.</span></span> <span data-ttu-id="a1352-177">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-177">Not nullable.</span></span> |
|<span data-ttu-id="a1352-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="a1352-178">orgRestrictions</span></span>|<span data-ttu-id="a1352-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a1352-179">String collection</span></span>| <span data-ttu-id="a1352-180">Организационное Тенантидс, к которому приложение ограничено.</span><span class="sxs-lookup"><span data-stu-id="a1352-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="a1352-181">Если коллекция пуста, приложение является несколькими клиентами (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="a1352-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="a1352-182">Если коллекция содержит Тенантидс, приложение ограничено Тенантидс Организации в коллекции.</span><span class="sxs-lookup"><span data-stu-id="a1352-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="a1352-183">Указание других клиентов, кроме tenantId, где зарегистрировано приложение, предполагает косвенное включение собственного tenantId приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="a1352-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="a1352-184">passwordCredentials</span></span>|<span data-ttu-id="a1352-185">Коллекция [passwordCredential](../resources/passwordcredential.md)</span><span class="sxs-lookup"><span data-stu-id="a1352-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="a1352-186">Коллекция учетных данных паролей, связанных с приложением.</span><span class="sxs-lookup"><span data-stu-id="a1352-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="a1352-187">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-187">Not nullable.</span></span>|
|<span data-ttu-id="a1352-188">Преаусоризедаппликатионс</span><span class="sxs-lookup"><span data-stu-id="a1352-188">preAuthorizedApplications</span></span>|<span data-ttu-id="a1352-189">Коллекция [preAuthorizedApplication](../resources/preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="a1352-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="a1352-190">Перечисляет приложения и запрашиваемые разрешения для неявного согласия.</span><span class="sxs-lookup"><span data-stu-id="a1352-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="a1352-191">Необходимо, чтобы администратор предоставил согласие на применение приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="a1352-192">Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="a1352-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="a1352-193">Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1352-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="a1352-194">Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1352-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="a1352-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="a1352-195">requiredResourceAccess</span></span>|<span data-ttu-id="a1352-196">Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md)</span><span class="sxs-lookup"><span data-stu-id="a1352-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="a1352-197">Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a1352-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="a1352-198">Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия.</span><span class="sxs-lookup"><span data-stu-id="a1352-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="a1352-199">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a1352-199">Not nullable.</span></span>|
|<span data-ttu-id="a1352-200">tags</span><span class="sxs-lookup"><span data-stu-id="a1352-200">tags</span></span>|<span data-ttu-id="a1352-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a1352-201">String collection</span></span>| <span data-ttu-id="a1352-202">Настраиваемые строки, которые можно использовать для классификации и определения приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="a1352-203">web</span><span class="sxs-lookup"><span data-stu-id="a1352-203">web</span></span>|[<span data-ttu-id="a1352-204">webApplication</span><span class="sxs-lookup"><span data-stu-id="a1352-204">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="a1352-205">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a1352-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="a1352-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1352-206">Response</span></span>

<span data-ttu-id="a1352-207">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1352-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1352-208">Пример</span><span class="sxs-lookup"><span data-stu-id="a1352-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1352-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1352-209">Request</span></span>
<span data-ttu-id="a1352-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1352-210">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1352-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1352-211">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1352-212">C#</span><span class="sxs-lookup"><span data-stu-id="a1352-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1352-213">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1352-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1352-214">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a1352-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a1352-215">Java</span><span class="sxs-lookup"><span data-stu-id="a1352-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a1352-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1352-216">Response</span></span>
<span data-ttu-id="a1352-217">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a1352-217">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
