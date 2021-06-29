---
title: тип ресурса resourceSpecificPermissionGrant
description: Указывает разрешение, которое имеет определенное приложение Azure AD.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fd6e9e09a092719f20de2c34f2120537cd00606
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162198"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="3f96c-103">тип ресурса resourceSpecificPermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3f96c-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="3f96c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f96c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f96c-105">РесурсSpecificPermissionGrant объявляет разрешение, предоставленное конкретному приложению AzureAD для экземпляра ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3f96c-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="3f96c-106">Дополнительные сведения о предоставлении приложениям согласия на доступ к конкретному экземпляру ресурса см. в примере " Согласие на [доступ к ресурсам".](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)</span><span class="sxs-lookup"><span data-stu-id="3f96c-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="3f96c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3f96c-107">Methods</span></span>

|  <span data-ttu-id="3f96c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3f96c-108">Method</span></span>                                                                   |  <span data-ttu-id="3f96c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3f96c-109">Return Type</span></span>                                                                     | <span data-ttu-id="3f96c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f96c-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="3f96c-111">Перечисление предоставленных разрешений группы</span><span class="sxs-lookup"><span data-stu-id="3f96c-111">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="3f96c-112">Коллекция [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="3f96c-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="3f96c-113">Список разрешений, определенных для ресурсов, которые были предоставлены в определенной [группе.](group.md)</span><span class="sxs-lookup"><span data-stu-id="3f96c-113">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="3f96c-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f96c-114">Properties</span></span>

| <span data-ttu-id="3f96c-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f96c-115">Property</span></span>        | <span data-ttu-id="3f96c-116">Тип</span><span class="sxs-lookup"><span data-stu-id="3f96c-116">Type</span></span>          | <span data-ttu-id="3f96c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3f96c-117">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="3f96c-118">id</span><span class="sxs-lookup"><span data-stu-id="3f96c-118">id</span></span>              | <span data-ttu-id="3f96c-119">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-119">string</span></span>        | <span data-ttu-id="3f96c-120">Уникальный идентификатор гранта разрешений, определяемого конкретными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="3f96c-120">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="3f96c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-121">Read-only.</span></span>           |
| <span data-ttu-id="3f96c-122">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f96c-122">deletedDateTime</span></span> | <span data-ttu-id="3f96c-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f96c-123">dateTimeOffset</span></span>| <span data-ttu-id="3f96c-124">Не используется.</span><span class="sxs-lookup"><span data-stu-id="3f96c-124">Not used.</span></span>                                                                             |
| <span data-ttu-id="3f96c-125">clientId</span><span class="sxs-lookup"><span data-stu-id="3f96c-125">clientId</span></span>        | <span data-ttu-id="3f96c-126">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-126">string</span></span>        | <span data-ttu-id="3f96c-127">ID приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="3f96c-127">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="3f96c-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-128">Read-only.</span></span>                            |
| <span data-ttu-id="3f96c-129">clientAppId</span><span class="sxs-lookup"><span data-stu-id="3f96c-129">clientAppId</span></span>     | <span data-ttu-id="3f96c-130">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-130">string</span></span>        | <span data-ttu-id="3f96c-131">ID директора службы приложения Azure AD, которое было предоставлено доступ.</span><span class="sxs-lookup"><span data-stu-id="3f96c-131">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="3f96c-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-132">Read-only.</span></span>   |
| <span data-ttu-id="3f96c-133">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="3f96c-133">resourceAppId</span></span>   | <span data-ttu-id="3f96c-134">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-134">string</span></span>        | <span data-ttu-id="3f96c-135">ID приложения Azure AD, на который размещен ресурс.</span><span class="sxs-lookup"><span data-stu-id="3f96c-135">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="3f96c-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-136">Read-only.</span></span>                        |
| <span data-ttu-id="3f96c-137">permissionType</span><span class="sxs-lookup"><span data-stu-id="3f96c-137">permissionType</span></span>  | <span data-ttu-id="3f96c-138">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-138">string</span></span>        | <span data-ttu-id="3f96c-139">Тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-139">The type of permission.</span></span> <span data-ttu-id="3f96c-140">Возможные значения: `Application`, `Delegated`.</span><span class="sxs-lookup"><span data-stu-id="3f96c-140">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="3f96c-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-141">Read-only.</span></span> |
| <span data-ttu-id="3f96c-142">разрешение</span><span class="sxs-lookup"><span data-stu-id="3f96c-142">permission</span></span>      | <span data-ttu-id="3f96c-143">string</span><span class="sxs-lookup"><span data-stu-id="3f96c-143">string</span></span>        | <span data-ttu-id="3f96c-144">Имя разрешения, определенного для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3f96c-144">The name of the resource-specific permission.</span></span> <span data-ttu-id="3f96c-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f96c-145">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="3f96c-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f96c-146">JSON representation</span></span>

<span data-ttu-id="3f96c-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f96c-147">The following is a JSON representation of the resource.</span></span>

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