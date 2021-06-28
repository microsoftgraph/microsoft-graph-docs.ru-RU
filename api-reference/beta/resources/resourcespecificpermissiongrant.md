---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f100d5658b2ecdc07daf928594180b0ce6129594
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162226"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="5c583-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5c583-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="5c583-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c583-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c583-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5c583-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="5c583-106">Дополнительные сведения о предоставлении приложениям согласия на доступ к конкретному экземпляру ресурса см. в примере " Согласие на [доступ к ресурсам".](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)</span><span class="sxs-lookup"><span data-stu-id="5c583-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="5c583-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5c583-107">Methods</span></span>

|  <span data-ttu-id="5c583-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5c583-108">Method</span></span>                                                                   |  <span data-ttu-id="5c583-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c583-109">Return Type</span></span>                                                                     | <span data-ttu-id="5c583-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c583-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="5c583-111">Список предоставленных разрешений чата</span><span class="sxs-lookup"><span data-stu-id="5c583-111">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="5c583-112">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="5c583-113">Список разрешений, определенных для ресурсов, которые были предоставлены в определенном [чате.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-113">List resource-specific permissions that have been granted in a specific [chat](chat.md).</span></span>  |
|[<span data-ttu-id="5c583-114">Список предоставленных разрешений группы</span><span class="sxs-lookup"><span data-stu-id="5c583-114">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="5c583-115">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-115">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="5c583-116">Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](group.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-116">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |
|[<span data-ttu-id="5c583-117">Перечисление предоставленных разрешений команды</span><span class="sxs-lookup"><span data-stu-id="5c583-117">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md) | <span data-ttu-id="5c583-118">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-118">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="5c583-119">Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](team.md)</span><span class="sxs-lookup"><span data-stu-id="5c583-119">List resource-specific permissions that have been granted in a specific [team](team.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="5c583-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c583-120">Properties</span></span>

| <span data-ttu-id="5c583-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c583-121">Property</span></span>        | <span data-ttu-id="5c583-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5c583-122">Type</span></span>          | <span data-ttu-id="5c583-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c583-123">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="5c583-124">id</span><span class="sxs-lookup"><span data-stu-id="5c583-124">id</span></span>              | <span data-ttu-id="5c583-125">string</span><span class="sxs-lookup"><span data-stu-id="5c583-125">string</span></span>        | <span data-ttu-id="5c583-126">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="5c583-126">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="5c583-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-127">Read-only.</span></span>           |
| <span data-ttu-id="5c583-128">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c583-128">deletedDateTime</span></span> | <span data-ttu-id="5c583-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c583-129">dateTimeOffset</span></span>| <span data-ttu-id="5c583-130">Не используется.</span><span class="sxs-lookup"><span data-stu-id="5c583-130">Not used.</span></span>                                                                             |
| <span data-ttu-id="5c583-131">clientId</span><span class="sxs-lookup"><span data-stu-id="5c583-131">clientId</span></span>        | <span data-ttu-id="5c583-132">string</span><span class="sxs-lookup"><span data-stu-id="5c583-132">string</span></span>        | <span data-ttu-id="5c583-133">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="5c583-133">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="5c583-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-134">Read-only.</span></span>                            |
| <span data-ttu-id="5c583-135">clientAppId</span><span class="sxs-lookup"><span data-stu-id="5c583-135">clientAppId</span></span>     | <span data-ttu-id="5c583-136">string</span><span class="sxs-lookup"><span data-stu-id="5c583-136">string</span></span>        | <span data-ttu-id="5c583-137">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="5c583-137">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="5c583-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-138">Read-only.</span></span>   |
| <span data-ttu-id="5c583-139">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="5c583-139">resourceAppId</span></span>   | <span data-ttu-id="5c583-140">string</span><span class="sxs-lookup"><span data-stu-id="5c583-140">string</span></span>        | <span data-ttu-id="5c583-141">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="5c583-141">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="5c583-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-142">Read-only.</span></span>                        |
| <span data-ttu-id="5c583-143">permissionType</span><span class="sxs-lookup"><span data-stu-id="5c583-143">permissionType</span></span>  | <span data-ttu-id="5c583-144">string</span><span class="sxs-lookup"><span data-stu-id="5c583-144">string</span></span>        | <span data-ttu-id="5c583-145">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="5c583-145">The type of permission.</span></span> <span data-ttu-id="5c583-146">Возможные значения: `Application`, `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="5c583-146">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="5c583-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-147">Read-only.</span></span> |
| <span data-ttu-id="5c583-148">разрешение</span><span class="sxs-lookup"><span data-stu-id="5c583-148">permission</span></span>      | <span data-ttu-id="5c583-149">string</span><span class="sxs-lookup"><span data-stu-id="5c583-149">string</span></span>        | <span data-ttu-id="5c583-150">Имя разрешения, определенного для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5c583-150">The name of the resource-specific permission.</span></span> <span data-ttu-id="5c583-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c583-151">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="5c583-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c583-152">JSON representation</span></span>

<span data-ttu-id="5c583-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c583-153">The following is a JSON representation of the resource.</span></span>

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


