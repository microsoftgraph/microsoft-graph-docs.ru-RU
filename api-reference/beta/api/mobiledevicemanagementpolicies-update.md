---
title: Обновление mobileDeviceManagementPolicy
description: Обновление свойств объекта управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 44c3424e3b2b179d3342b06ff4f40824e8055c89
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440675"
---
# <a name="update-mobiledevicemanagementpolicy"></a><span data-ttu-id="36918-103">Обновление mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="36918-103">Update mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="36918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36918-105">Обновление свойств объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="36918-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36918-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36918-106">Permissions</span></span>

<span data-ttu-id="36918-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36918-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36918-109">Permission type</span></span>|<span data-ttu-id="36918-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36918-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36918-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36918-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36918-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="36918-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="36918-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36918-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36918-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36918-114">Not supported.</span></span>|
|<span data-ttu-id="36918-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36918-115">Application</span></span> | <span data-ttu-id="36918-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36918-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36918-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36918-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="36918-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36918-118">Request headers</span></span>

|<span data-ttu-id="36918-119">Имя</span><span class="sxs-lookup"><span data-stu-id="36918-119">Name</span></span>|<span data-ttu-id="36918-120">Описание</span><span class="sxs-lookup"><span data-stu-id="36918-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36918-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36918-121">Authorization</span></span>|<span data-ttu-id="36918-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36918-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="36918-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36918-124">Content-Type</span></span>|<span data-ttu-id="36918-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36918-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36918-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36918-127">Request body</span></span>

<span data-ttu-id="36918-128">В теле запроса поставляем JSON-представление объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="36918-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="36918-129">В теле запроса укажи значения для перечисленных ниже полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="36918-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="36918-130">**Примечание:** С другими свойствами нельзя использовать `PATCH` `appliesTo` операцию.</span><span class="sxs-lookup"><span data-stu-id="36918-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="36918-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="36918-131">Property</span></span>|<span data-ttu-id="36918-132">Тип</span><span class="sxs-lookup"><span data-stu-id="36918-132">Type</span></span>|<span data-ttu-id="36918-133">Описание</span><span class="sxs-lookup"><span data-stu-id="36918-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36918-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="36918-134">appliesTo</span></span>|<span data-ttu-id="36918-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="36918-135">policyScope</span></span>|<span data-ttu-id="36918-136">Определяет группы, к которые применяется этот параметр политики.</span><span class="sxs-lookup"><span data-stu-id="36918-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="36918-137">Возможные значения: `none` , `all` , `selected` **Важно: не** может использоваться при `selected` указании этого свойства.</span><span class="sxs-lookup"><span data-stu-id="36918-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="36918-138">Используйте [includedGroups для](../api/mobiledevicemanagementpolicies-post-includedgroups.md) добавления определенных групп.</span><span class="sxs-lookup"><span data-stu-id="36918-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) to add specific groups.</span></span> <span data-ttu-id="36918-139">Использование `all` удаляет все существующие группы.</span><span class="sxs-lookup"><span data-stu-id="36918-139">Using `all` will remove any existing groups.</span></span>|
|<span data-ttu-id="36918-140">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="36918-140">complianceUrl</span></span>|<span data-ttu-id="36918-141">String</span><span class="sxs-lookup"><span data-stu-id="36918-141">String</span></span>|<span data-ttu-id="36918-142">URL-адрес соответствия приложению управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="36918-142">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="36918-143">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="36918-143">discoveryUrl</span></span>|<span data-ttu-id="36918-144">String</span><span class="sxs-lookup"><span data-stu-id="36918-144">String</span></span>|<span data-ttu-id="36918-145">Обнаружение URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="36918-145">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="36918-146">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="36918-146">termsOfUseUrl</span></span>|<span data-ttu-id="36918-147">String</span><span class="sxs-lookup"><span data-stu-id="36918-147">String</span></span>|<span data-ttu-id="36918-148">Условия использования URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="36918-148">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="36918-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="36918-149">Response</span></span>

<span data-ttu-id="36918-150">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="36918-150">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36918-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="36918-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36918-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="36918-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36918-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="36918-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```
# <a name="c"></a>[<span data-ttu-id="36918-154">C#</span><span class="sxs-lookup"><span data-stu-id="36918-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36918-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36918-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36918-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36918-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36918-157">Java</span><span class="sxs-lookup"><span data-stu-id="36918-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36918-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="36918-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
