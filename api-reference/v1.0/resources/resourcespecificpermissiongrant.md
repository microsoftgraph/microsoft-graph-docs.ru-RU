---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769c4d405473ef800b92fbecb8797588cf59eb57
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944304"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="49e7d-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="49e7d-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="49e7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49e7d-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49e7d-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="49e7d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="49e7d-106">Methods</span></span>

|  <span data-ttu-id="49e7d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="49e7d-107">Method</span></span>                                                                   |  <span data-ttu-id="49e7d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="49e7d-108">Return Type</span></span>                                                                     | <span data-ttu-id="49e7d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="49e7d-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="49e7d-110">Список разрешений группы</span><span class="sxs-lookup"><span data-stu-id="49e7d-110">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="49e7d-111">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="49e7d-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="49e7d-112">Список разрешений, предоставленных в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="49e7d-112">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="49e7d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="49e7d-113">Properties</span></span>

| <span data-ttu-id="49e7d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="49e7d-114">Property</span></span>        | <span data-ttu-id="49e7d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="49e7d-115">Type</span></span>          | <span data-ttu-id="49e7d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="49e7d-116">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="49e7d-117">id</span><span class="sxs-lookup"><span data-stu-id="49e7d-117">id</span></span>              | <span data-ttu-id="49e7d-118">string</span><span class="sxs-lookup"><span data-stu-id="49e7d-118">string</span></span>        | <span data-ttu-id="49e7d-119">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="49e7d-119">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="49e7d-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-120">Read-only.</span></span>           |
| <span data-ttu-id="49e7d-121">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="49e7d-121">deletedDateTime</span></span> | <span data-ttu-id="49e7d-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e7d-122">dateTimeOffset</span></span>| <span data-ttu-id="49e7d-123">Не используется.</span><span class="sxs-lookup"><span data-stu-id="49e7d-123">Not used.</span></span>                                                                             |
| <span data-ttu-id="49e7d-124">clientId</span><span class="sxs-lookup"><span data-stu-id="49e7d-124">clientId</span></span>        | <span data-ttu-id="49e7d-125">String</span><span class="sxs-lookup"><span data-stu-id="49e7d-125">string</span></span>        | <span data-ttu-id="49e7d-126">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="49e7d-126">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="49e7d-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-127">Read-only.</span></span>                            |
| <span data-ttu-id="49e7d-128">clientAppId</span><span class="sxs-lookup"><span data-stu-id="49e7d-128">clientAppId</span></span>     | <span data-ttu-id="49e7d-129">String</span><span class="sxs-lookup"><span data-stu-id="49e7d-129">string</span></span>        | <span data-ttu-id="49e7d-130">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="49e7d-130">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="49e7d-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-131">Read-only.</span></span>   |
| <span data-ttu-id="49e7d-132">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="49e7d-132">resourceAppId</span></span>   | <span data-ttu-id="49e7d-133">String</span><span class="sxs-lookup"><span data-stu-id="49e7d-133">string</span></span>        | <span data-ttu-id="49e7d-134">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="49e7d-134">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="49e7d-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-135">Read-only.</span></span>                        |
| <span data-ttu-id="49e7d-136">permissionType</span><span class="sxs-lookup"><span data-stu-id="49e7d-136">permissionType</span></span>  | <span data-ttu-id="49e7d-137">String</span><span class="sxs-lookup"><span data-stu-id="49e7d-137">string</span></span>        | <span data-ttu-id="49e7d-138">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-138">The type of permission.</span></span> <span data-ttu-id="49e7d-139">Возможные значения: `Application`, `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="49e7d-139">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="49e7d-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-140">Read-only.</span></span> |
| <span data-ttu-id="49e7d-141">разрешение</span><span class="sxs-lookup"><span data-stu-id="49e7d-141">permission</span></span>      | <span data-ttu-id="49e7d-142">String</span><span class="sxs-lookup"><span data-stu-id="49e7d-142">string</span></span>        | <span data-ttu-id="49e7d-143">Имя разрешения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-143">The name of the permission.</span></span> <span data-ttu-id="49e7d-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e7d-144">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="49e7d-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49e7d-145">JSON representation</span></span>

<span data-ttu-id="49e7d-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49e7d-146">The following is a JSON representation of the resource.</span></span>

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