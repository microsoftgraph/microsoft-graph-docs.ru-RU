---
title: Обновление mobileAppManagementPolicy
description: Обновление свойств объекта политики управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b553a291ce986a3084403c55f3c991fb260c4828
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401647"
---
# <a name="update-mobileappmanagementpolicy"></a><span data-ttu-id="0f7d6-103">Обновление mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="0f7d6-103">Update mobileAppManagementPolicy</span></span>

<span data-ttu-id="0f7d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f7d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f7d6-105">Обновление свойств объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f7d6-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f7d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f7d6-106">Permissions</span></span>

<span data-ttu-id="0f7d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f7d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f7d6-109">Permission type</span></span>|<span data-ttu-id="0f7d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f7d6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f7d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f7d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f7d6-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="0f7d6-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="0f7d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f7d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f7d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-114">Not supported.</span></span>|
|<span data-ttu-id="0f7d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f7d6-115">Application</span></span> | <span data-ttu-id="0f7d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f7d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f7d6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f7d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f7d6-118">Request headers</span></span>

|<span data-ttu-id="0f7d6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0f7d6-119">Name</span></span>|<span data-ttu-id="0f7d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7d6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f7d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f7d6-121">Authorization</span></span>|<span data-ttu-id="0f7d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0f7d6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f7d6-124">Content-Type</span></span>|<span data-ttu-id="0f7d6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f7d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f7d6-127">Request body</span></span>

<span data-ttu-id="0f7d6-128">В теле запроса поставляем JSON-представление объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f7d6-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="0f7d6-129">В теле запроса укажи значения для перечисленных ниже полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="0f7d6-130">**Примечание:** С другими свойствами нельзя использовать `PATCH` `appliesTo` операцию.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="0f7d6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f7d6-131">Property</span></span>|<span data-ttu-id="0f7d6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0f7d6-132">Type</span></span>|<span data-ttu-id="0f7d6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7d6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f7d6-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0f7d6-134">appliesTo</span></span>|<span data-ttu-id="0f7d6-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="0f7d6-135">policyScope</span></span>|<span data-ttu-id="0f7d6-136">Определяет группы, к которые применяется этот параметр политики.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="0f7d6-137">Возможные значения: `none` , `all` , `selected` **Важно: не** может использоваться при `selected` указании этого свойства.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="0f7d6-138">Используйте [includedGroups для](../api/mobileappmanagementpolicies-post-includedgroups.md) добавления определенных групп.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-138">Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) to add specific groups.</span></span>|
|<span data-ttu-id="0f7d6-139">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="0f7d6-139">complianceUrl</span></span>|<span data-ttu-id="0f7d6-140">String</span><span class="sxs-lookup"><span data-stu-id="0f7d6-140">String</span></span>|<span data-ttu-id="0f7d6-141">URL-адрес соответствия приложению управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="0f7d6-141">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="0f7d6-142">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="0f7d6-142">discoveryUrl</span></span>|<span data-ttu-id="0f7d6-143">String</span><span class="sxs-lookup"><span data-stu-id="0f7d6-143">String</span></span>|<span data-ttu-id="0f7d6-144">Обнаружение URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="0f7d6-144">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="0f7d6-145">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="0f7d6-145">termsOfUseUrl</span></span>|<span data-ttu-id="0f7d6-146">String</span><span class="sxs-lookup"><span data-stu-id="0f7d6-146">String</span></span>|<span data-ttu-id="0f7d6-147">Условия использования URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="0f7d6-147">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="0f7d6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f7d6-148">Response</span></span>

<span data-ttu-id="0f7d6-149">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0f7d6-149">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f7d6-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="0f7d6-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f7d6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f7d6-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.mg.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.mg.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a><span data-ttu-id="0f7d6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f7d6-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
