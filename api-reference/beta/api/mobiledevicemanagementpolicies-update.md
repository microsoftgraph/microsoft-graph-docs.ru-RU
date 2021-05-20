---
title: Обновление mobileDeviceManagementPolicy
description: Обновление свойств объекта управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 112c76fbb240e8ff30b47b47de3f6d2966af8a11
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547431"
---
# <a name="update-mobiledevicemanagementpolicy"></a><span data-ttu-id="6c497-103">Обновление mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="6c497-103">Update mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="6c497-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c497-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c497-105">Обновление свойств объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c497-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c497-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c497-106">Permissions</span></span>

<span data-ttu-id="6c497-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c497-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c497-109">Permission type</span></span>|<span data-ttu-id="6c497-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c497-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c497-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c497-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c497-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c497-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="6c497-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c497-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c497-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c497-114">Not supported.</span></span>|
|<span data-ttu-id="6c497-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c497-115">Application</span></span> | <span data-ttu-id="6c497-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c497-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c497-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c497-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6c497-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c497-118">Request headers</span></span>

|<span data-ttu-id="6c497-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c497-119">Name</span></span>|<span data-ttu-id="6c497-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c497-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c497-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c497-121">Authorization</span></span>|<span data-ttu-id="6c497-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c497-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6c497-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c497-124">Content-Type</span></span>|<span data-ttu-id="6c497-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c497-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c497-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c497-127">Request body</span></span>

<span data-ttu-id="6c497-128">В теле запроса поставляем JSON-представление объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c497-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="6c497-129">В теле запроса укажи значения для перечисленных ниже полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="6c497-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="6c497-130">**Примечание:** С другими свойствами нельзя использовать `PATCH` `appliesTo` операцию.</span><span class="sxs-lookup"><span data-stu-id="6c497-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="6c497-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c497-131">Property</span></span>|<span data-ttu-id="6c497-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6c497-132">Type</span></span>|<span data-ttu-id="6c497-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6c497-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c497-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="6c497-134">appliesTo</span></span>|<span data-ttu-id="6c497-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="6c497-135">policyScope</span></span>|<span data-ttu-id="6c497-136">Определяет группы, к которые применяется этот параметр политики.</span><span class="sxs-lookup"><span data-stu-id="6c497-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="6c497-137">Возможные значения: `none` , `all` , `selected` **Важно: не** может использоваться при `selected` указании этого свойства.</span><span class="sxs-lookup"><span data-stu-id="6c497-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="6c497-138">Используйте [includedGroups для](../api/mobiledevicemanagementpolicies-post-includedgroups.md) добавления определенных групп.</span><span class="sxs-lookup"><span data-stu-id="6c497-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) to add specific groups.</span></span> <span data-ttu-id="6c497-139">Использование `all` удаляет все существующие группы.</span><span class="sxs-lookup"><span data-stu-id="6c497-139">Using `all` will remove any existing groups.</span></span>|
|<span data-ttu-id="6c497-140">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="6c497-140">complianceUrl</span></span>|<span data-ttu-id="6c497-141">String</span><span class="sxs-lookup"><span data-stu-id="6c497-141">String</span></span>|<span data-ttu-id="6c497-142">URL-адрес соответствия приложению управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="6c497-142">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="6c497-143">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="6c497-143">discoveryUrl</span></span>|<span data-ttu-id="6c497-144">String</span><span class="sxs-lookup"><span data-stu-id="6c497-144">String</span></span>|<span data-ttu-id="6c497-145">Обнаружение URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="6c497-145">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="6c497-146">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="6c497-146">termsOfUseUrl</span></span>|<span data-ttu-id="6c497-147">String</span><span class="sxs-lookup"><span data-stu-id="6c497-147">String</span></span>|<span data-ttu-id="6c497-148">Условия использования URL-адреса приложения для управления мобильностью</span><span class="sxs-lookup"><span data-stu-id="6c497-148">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="6c497-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c497-149">Response</span></span>

<span data-ttu-id="6c497-150">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6c497-150">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c497-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c497-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c497-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c497-152">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="6c497-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c497-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
