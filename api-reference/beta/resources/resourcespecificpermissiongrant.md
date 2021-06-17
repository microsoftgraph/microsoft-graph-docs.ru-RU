---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 56d7ea203f4ed72f45a3650197c1484f817567e6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992319"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="e6c59-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e6c59-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="e6c59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6c59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c59-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e6c59-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="e6c59-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e6c59-106">Methods</span></span>

|  <span data-ttu-id="e6c59-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e6c59-107">Method</span></span>                                                                   |  <span data-ttu-id="e6c59-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6c59-108">Return Type</span></span>                                                                     | <span data-ttu-id="e6c59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c59-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="e6c59-110">Список разрешений чата</span><span class="sxs-lookup"><span data-stu-id="e6c59-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="e6c59-111">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="e6c59-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="e6c59-112">Список разрешений, предоставленных в определенном чате.</span><span class="sxs-lookup"><span data-stu-id="e6c59-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="e6c59-113">Список разрешений группы</span><span class="sxs-lookup"><span data-stu-id="e6c59-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="e6c59-114">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="e6c59-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="e6c59-115">Список разрешений, предоставленных в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="e6c59-115">List permissions that have been granted in a specific group.</span></span> |
|[<span data-ttu-id="e6c59-116">Список разрешений группы</span><span class="sxs-lookup"><span data-stu-id="e6c59-116">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md)   | <span data-ttu-id="e6c59-117">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="e6c59-117">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="e6c59-118">Список разрешений, предоставленных в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="e6c59-118">List permissions that have been granted in a specific team.</span></span>  |

## <a name="properties"></a><span data-ttu-id="e6c59-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6c59-119">Properties</span></span>

| <span data-ttu-id="e6c59-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6c59-120">Property</span></span>        | <span data-ttu-id="e6c59-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e6c59-121">Type</span></span>          | <span data-ttu-id="e6c59-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c59-122">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e6c59-123">id</span><span class="sxs-lookup"><span data-stu-id="e6c59-123">id</span></span>              | <span data-ttu-id="e6c59-124">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-124">string</span></span>        | <span data-ttu-id="e6c59-125">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="e6c59-125">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="e6c59-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-126">Read-only.</span></span>           |
| <span data-ttu-id="e6c59-127">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6c59-127">deletedDateTime</span></span> | <span data-ttu-id="e6c59-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6c59-128">dateTimeOffset</span></span>| <span data-ttu-id="e6c59-129">Не используется.</span><span class="sxs-lookup"><span data-stu-id="e6c59-129">Not used.</span></span>                                                                             |
| <span data-ttu-id="e6c59-130">clientId</span><span class="sxs-lookup"><span data-stu-id="e6c59-130">clientId</span></span>        | <span data-ttu-id="e6c59-131">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-131">string</span></span>        | <span data-ttu-id="e6c59-132">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="e6c59-132">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e6c59-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-133">Read-only.</span></span>                            |
| <span data-ttu-id="e6c59-134">clientAppId</span><span class="sxs-lookup"><span data-stu-id="e6c59-134">clientAppId</span></span>     | <span data-ttu-id="e6c59-135">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-135">string</span></span>        | <span data-ttu-id="e6c59-136">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="e6c59-136">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e6c59-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-137">Read-only.</span></span>   |
| <span data-ttu-id="e6c59-138">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="e6c59-138">resourceAppId</span></span>   | <span data-ttu-id="e6c59-139">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-139">string</span></span>        | <span data-ttu-id="e6c59-140">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="e6c59-140">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="e6c59-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-141">Read-only.</span></span>                        |
| <span data-ttu-id="e6c59-142">permissionType</span><span class="sxs-lookup"><span data-stu-id="e6c59-142">permissionType</span></span>  | <span data-ttu-id="e6c59-143">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-143">string</span></span>        | <span data-ttu-id="e6c59-144">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-144">The type of permission.</span></span> <span data-ttu-id="e6c59-145">Возможные значения: `Application`, `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="e6c59-145">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="e6c59-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-146">Read-only.</span></span> |
| <span data-ttu-id="e6c59-147">разрешение</span><span class="sxs-lookup"><span data-stu-id="e6c59-147">permission</span></span>      | <span data-ttu-id="e6c59-148">string</span><span class="sxs-lookup"><span data-stu-id="e6c59-148">string</span></span>        | <span data-ttu-id="e6c59-149">Имя разрешения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-149">The name of the permission.</span></span> <span data-ttu-id="e6c59-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6c59-150">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="e6c59-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6c59-151">JSON representation</span></span>

<span data-ttu-id="e6c59-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6c59-152">The following is a JSON representation of the resource.</span></span>

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


