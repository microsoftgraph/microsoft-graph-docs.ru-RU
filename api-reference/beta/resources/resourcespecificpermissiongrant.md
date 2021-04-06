---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34faa7a7b709d85cd2bee3208cc22270fecbe74
ms.sourcegitcommit: 8b1a6d7b0516f936ce4626246408f067527f5082
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2021
ms.locfileid: "51594913"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="78ce5-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="78ce5-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="78ce5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78ce5-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="78ce5-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="78ce5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="78ce5-106">Methods</span></span>

|  <span data-ttu-id="78ce5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="78ce5-107">Method</span></span>                                                                   |  <span data-ttu-id="78ce5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78ce5-108">Return Type</span></span>                                                                     | <span data-ttu-id="78ce5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78ce5-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="78ce5-110">Список разрешений чата</span><span class="sxs-lookup"><span data-stu-id="78ce5-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="78ce5-111">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="78ce5-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="78ce5-112">Список разрешений, предоставленных в определенном чате.</span><span class="sxs-lookup"><span data-stu-id="78ce5-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="78ce5-113">Список разрешений группы</span><span class="sxs-lookup"><span data-stu-id="78ce5-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="78ce5-114">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="78ce5-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="78ce5-115">Список разрешений, предоставленных в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="78ce5-115">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="78ce5-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="78ce5-116">Properties</span></span>

| <span data-ttu-id="78ce5-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="78ce5-117">Property</span></span>        | <span data-ttu-id="78ce5-118">Тип</span><span class="sxs-lookup"><span data-stu-id="78ce5-118">Type</span></span>          | <span data-ttu-id="78ce5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="78ce5-119">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="78ce5-120">id</span><span class="sxs-lookup"><span data-stu-id="78ce5-120">id</span></span>              | <span data-ttu-id="78ce5-121">string</span><span class="sxs-lookup"><span data-stu-id="78ce5-121">string</span></span>        | <span data-ttu-id="78ce5-122">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="78ce5-122">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="78ce5-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-123">Read-only.</span></span>           |
| <span data-ttu-id="78ce5-124">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="78ce5-124">deletedDateTime</span></span> | <span data-ttu-id="78ce5-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ce5-125">dateTimeOffset</span></span>| <span data-ttu-id="78ce5-126">Не используется.</span><span class="sxs-lookup"><span data-stu-id="78ce5-126">Not used.</span></span>                                                                             |
| <span data-ttu-id="78ce5-127">clientId</span><span class="sxs-lookup"><span data-stu-id="78ce5-127">clientId</span></span>        | <span data-ttu-id="78ce5-128">Строка</span><span class="sxs-lookup"><span data-stu-id="78ce5-128">string</span></span>        | <span data-ttu-id="78ce5-129">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="78ce5-129">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="78ce5-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-130">Read-only.</span></span>                            |
| <span data-ttu-id="78ce5-131">clientAppId</span><span class="sxs-lookup"><span data-stu-id="78ce5-131">clientAppId</span></span>     | <span data-ttu-id="78ce5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="78ce5-132">string</span></span>        | <span data-ttu-id="78ce5-133">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="78ce5-133">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="78ce5-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-134">Read-only.</span></span>   |
| <span data-ttu-id="78ce5-135">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="78ce5-135">resourceAppId</span></span>   | <span data-ttu-id="78ce5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="78ce5-136">string</span></span>        | <span data-ttu-id="78ce5-137">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="78ce5-137">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="78ce5-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-138">Read-only.</span></span>                        |
| <span data-ttu-id="78ce5-139">permissionType</span><span class="sxs-lookup"><span data-stu-id="78ce5-139">permissionType</span></span>  | <span data-ttu-id="78ce5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="78ce5-140">string</span></span>        | <span data-ttu-id="78ce5-141">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-141">The type of permission.</span></span> <span data-ttu-id="78ce5-142">Возможные значения: `Application` , `Delegated` .</span><span class="sxs-lookup"><span data-stu-id="78ce5-142">Possible values are: `Application`,`Delegated`.</span></span> <span data-ttu-id="78ce5-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-143">Read-only.</span></span> |
| <span data-ttu-id="78ce5-144">разрешение</span><span class="sxs-lookup"><span data-stu-id="78ce5-144">permission</span></span>      | <span data-ttu-id="78ce5-145">Строка</span><span class="sxs-lookup"><span data-stu-id="78ce5-145">string</span></span>        | <span data-ttu-id="78ce5-146">Имя разрешения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-146">The name of the permission.</span></span> <span data-ttu-id="78ce5-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78ce5-147">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="78ce5-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78ce5-148">JSON representation</span></span>

<span data-ttu-id="78ce5-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78ce5-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```


