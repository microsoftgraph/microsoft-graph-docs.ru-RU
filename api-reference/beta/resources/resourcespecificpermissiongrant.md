---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7119d25f25b0e4f382a077ca6a1264dc22e11d5b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765904"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="8e0f1-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e0f1-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="8e0f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e0f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e0f1-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="8e0f1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8e0f1-106">Methods</span></span>

|  <span data-ttu-id="8e0f1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8e0f1-107">Method</span></span>                                                                   |  <span data-ttu-id="8e0f1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e0f1-108">Return Type</span></span>                                                                     | <span data-ttu-id="8e0f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0f1-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="8e0f1-110">Список разрешений чата</span><span class="sxs-lookup"><span data-stu-id="8e0f1-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="8e0f1-111">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="8e0f1-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="8e0f1-112">Список разрешений, предоставленных в определенном чате.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="8e0f1-113">Список разрешений группы</span><span class="sxs-lookup"><span data-stu-id="8e0f1-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="8e0f1-114">[коллекция resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="8e0f1-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="8e0f1-115">Список разрешений, предоставленных в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-115">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e0f1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e0f1-116">Properties</span></span>

| <span data-ttu-id="8e0f1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e0f1-117">Property</span></span>        | <span data-ttu-id="8e0f1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0f1-118">Type</span></span>          | <span data-ttu-id="8e0f1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0f1-119">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8e0f1-120">id</span><span class="sxs-lookup"><span data-stu-id="8e0f1-120">id</span></span>              | <span data-ttu-id="8e0f1-121">string</span><span class="sxs-lookup"><span data-stu-id="8e0f1-121">string</span></span>        | <span data-ttu-id="8e0f1-122">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-122">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="8e0f1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-123">Read-only.</span></span>           |
| <span data-ttu-id="8e0f1-124">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0f1-124">deletedDateTime</span></span> | <span data-ttu-id="8e0f1-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0f1-125">dateTimeOffset</span></span>| <span data-ttu-id="8e0f1-126">Не используется.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-126">Not used.</span></span>                                                                             |
| <span data-ttu-id="8e0f1-127">clientId</span><span class="sxs-lookup"><span data-stu-id="8e0f1-127">clientId</span></span>        | <span data-ttu-id="8e0f1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="8e0f1-128">string</span></span>        | <span data-ttu-id="8e0f1-129">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-129">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="8e0f1-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-130">Read-only.</span></span>                            |
| <span data-ttu-id="8e0f1-131">clientAppId</span><span class="sxs-lookup"><span data-stu-id="8e0f1-131">clientAppId</span></span>     | <span data-ttu-id="8e0f1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8e0f1-132">string</span></span>        | <span data-ttu-id="8e0f1-133">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-133">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="8e0f1-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-134">Read-only.</span></span>   |
| <span data-ttu-id="8e0f1-135">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="8e0f1-135">resourceAppId</span></span>   | <span data-ttu-id="8e0f1-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8e0f1-136">string</span></span>        | <span data-ttu-id="8e0f1-137">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-137">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="8e0f1-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-138">Read-only.</span></span>                        |
| <span data-ttu-id="8e0f1-139">permissionType</span><span class="sxs-lookup"><span data-stu-id="8e0f1-139">permissionType</span></span>  | <span data-ttu-id="8e0f1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="8e0f1-140">string</span></span>        | <span data-ttu-id="8e0f1-141">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-141">The type of permission.</span></span> <span data-ttu-id="8e0f1-142">Возможные значения: `Application`, `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-142">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="8e0f1-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-143">Read-only.</span></span> |
| <span data-ttu-id="8e0f1-144">разрешение</span><span class="sxs-lookup"><span data-stu-id="8e0f1-144">permission</span></span>      | <span data-ttu-id="8e0f1-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8e0f1-145">string</span></span>        | <span data-ttu-id="8e0f1-146">Имя разрешения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-146">The name of the permission.</span></span> <span data-ttu-id="8e0f1-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-147">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="8e0f1-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e0f1-148">JSON representation</span></span>

<span data-ttu-id="8e0f1-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e0f1-149">The following is a JSON representation of the resource.</span></span>

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


