---
title: тип ресурса cloudPcAuditActor
description: Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c0c63e9e9d0db7a5227f0ab7b818c8ab3d3944d9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211348"
---
# <a name="cloudpcauditactor-resource-type"></a><span data-ttu-id="f3285-103">тип ресурса cloudPcAuditActor</span><span class="sxs-lookup"><span data-stu-id="f3285-103">cloudPcAuditActor resource type</span></span>

<span data-ttu-id="f3285-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3285-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3285-105">Субъект аудита, представленный пользователем Azure AD и приложением, связанным с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="f3285-105">The audit actor represented by the Azure AD user and application associated with the audit event.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="f3285-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3285-106">Properties</span></span>

|<span data-ttu-id="f3285-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3285-107">Property</span></span>|<span data-ttu-id="f3285-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f3285-108">Type</span></span>|<span data-ttu-id="f3285-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f3285-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3285-110">type</span><span class="sxs-lookup"><span data-stu-id="f3285-110">type</span></span>|[<span data-ttu-id="f3285-111">cloudPcAuditActorType</span><span class="sxs-lookup"><span data-stu-id="f3285-111">cloudPcAuditActorType</span></span>](#cloudpcauditactortype-values)|<span data-ttu-id="f3285-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="f3285-112">The actor type.</span></span> <span data-ttu-id="f3285-113">Возможные значения включают `ItPro` `Application` , и `Partner` `Unknown` .</span><span class="sxs-lookup"><span data-stu-id="f3285-113">Possible values include `ItPro`, `Application`, `Partner` and `Unknown`.</span></span>|
|<span data-ttu-id="f3285-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f3285-114">userPermissions</span></span>|<span data-ttu-id="f3285-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f3285-115">String collection</span></span>|<span data-ttu-id="f3285-116">Список разрешений пользователей и разрешений приложений при выполнении события аудита.</span><span class="sxs-lookup"><span data-stu-id="f3285-116">List of user permissions and application permissions when the audit event was performed.</span></span>|
|<span data-ttu-id="f3285-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="f3285-117">applicationId</span></span>|<span data-ttu-id="f3285-118">String</span><span class="sxs-lookup"><span data-stu-id="f3285-118">String</span></span>|<span data-ttu-id="f3285-119">ID приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3285-119">Azure AD application ID.</span></span>|
|<span data-ttu-id="f3285-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3285-120">applicationDisplayName</span></span>|<span data-ttu-id="f3285-121">String</span><span class="sxs-lookup"><span data-stu-id="f3285-121">String</span></span>|<span data-ttu-id="f3285-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f3285-122">Name of the application.</span></span>|
|<span data-ttu-id="f3285-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3285-123">userPrincipalName</span></span>|<span data-ttu-id="f3285-124">String</span><span class="sxs-lookup"><span data-stu-id="f3285-124">String</span></span>|<span data-ttu-id="f3285-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="f3285-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f3285-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3285-126">servicePrincipalName</span></span>|<span data-ttu-id="f3285-127">String</span><span class="sxs-lookup"><span data-stu-id="f3285-127">String</span></span>|<span data-ttu-id="f3285-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="f3285-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f3285-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f3285-129">ipAddress</span></span>|<span data-ttu-id="f3285-130">String</span><span class="sxs-lookup"><span data-stu-id="f3285-130">String</span></span>|<span data-ttu-id="f3285-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="f3285-131">IP address.</span></span>|
|<span data-ttu-id="f3285-132">userId</span><span class="sxs-lookup"><span data-stu-id="f3285-132">userId</span></span>|<span data-ttu-id="f3285-133">String</span><span class="sxs-lookup"><span data-stu-id="f3285-133">String</span></span>|<span data-ttu-id="f3285-134">ID пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3285-134">Azure AD user ID.</span></span>|
|<span data-ttu-id="f3285-135">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="f3285-135">userRoleScopeTags</span></span>|<span data-ttu-id="f3285-136">[коллекция cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="f3285-136">[cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md) collection</span></span>|<span data-ttu-id="f3285-137">Список тегов области ролей.</span><span class="sxs-lookup"><span data-stu-id="f3285-137">List of role scope tags.</span></span>|
|<span data-ttu-id="f3285-138">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="f3285-138">remoteTenantId</span></span>|<span data-ttu-id="f3285-139">String</span><span class="sxs-lookup"><span data-stu-id="f3285-139">String</span></span>|<span data-ttu-id="f3285-140">Делегированная ид клиента-партнера.</span><span class="sxs-lookup"><span data-stu-id="f3285-140">The delegated partner tenant ID.</span></span>|
|<span data-ttu-id="f3285-141">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="f3285-141">remoteUserId</span></span>|<span data-ttu-id="f3285-142">String</span><span class="sxs-lookup"><span data-stu-id="f3285-142">String</span></span>|<span data-ttu-id="f3285-143">Делегированная ид пользователя-партнера.</span><span class="sxs-lookup"><span data-stu-id="f3285-143">The delegated partner user ID.</span></span>|

### <a name="cloudpcauditactortype-values"></a><span data-ttu-id="f3285-144">значения cloudPcAuditActorType</span><span class="sxs-lookup"><span data-stu-id="f3285-144">cloudPcAuditActorType values</span></span>

|<span data-ttu-id="f3285-145">Member</span><span class="sxs-lookup"><span data-stu-id="f3285-145">Member</span></span>|<span data-ttu-id="f3285-146">Описание</span><span class="sxs-lookup"><span data-stu-id="f3285-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3285-147">itPro</span><span class="sxs-lookup"><span data-stu-id="f3285-147">itPro</span></span>|<span data-ttu-id="f3285-148">Операция была выполнена ИТ-профессионалом.</span><span class="sxs-lookup"><span data-stu-id="f3285-148">The operation was performed by an IT pro.</span></span>|
|<span data-ttu-id="f3285-149">приложение</span><span class="sxs-lookup"><span data-stu-id="f3285-149">application</span></span>|<span data-ttu-id="f3285-150">Операция была выполнена приложением.</span><span class="sxs-lookup"><span data-stu-id="f3285-150">The operation was performed by the application.</span></span>|
|<span data-ttu-id="f3285-151">партнер</span><span class="sxs-lookup"><span data-stu-id="f3285-151">partner</span></span>|<span data-ttu-id="f3285-152">Операция была выполнена партнером.</span><span class="sxs-lookup"><span data-stu-id="f3285-152">The operation was performed by a partner.</span></span>|
|<span data-ttu-id="f3285-153">unknown</span><span class="sxs-lookup"><span data-stu-id="f3285-153">unknown</span></span>|<span data-ttu-id="f3285-154">Неизвестный актер.</span><span class="sxs-lookup"><span data-stu-id="f3285-154">Unknown actor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3285-155">Связи</span><span class="sxs-lookup"><span data-stu-id="f3285-155">Relationships</span></span>

<span data-ttu-id="f3285-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3285-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3285-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3285-157">JSON Representation</span></span>

<span data-ttu-id="f3285-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3285-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
