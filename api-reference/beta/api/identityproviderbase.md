---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 71c6d58e9ad70773df39adc7d2a91393d64cd460
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491109"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="edbcd-103">Тип ресурса identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="edbcd-103">identityProviderBase resource type</span></span>
<span data-ttu-id="edbcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edbcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edbcd-105">Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="edbcd-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="edbcd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="edbcd-106">Methods</span></span>

| <span data-ttu-id="edbcd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="edbcd-107">Method</span></span>       | <span data-ttu-id="edbcd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="edbcd-108">Return Type</span></span>  |<span data-ttu-id="edbcd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="edbcd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="edbcd-110">Список</span><span class="sxs-lookup"><span data-stu-id="edbcd-110">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="edbcd-111">Коллекция identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="edbcd-111">identityProviderBase collection</span></span>|<span data-ttu-id="edbcd-112">Получение всех поставщиков удостоверений, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="edbcd-112">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="edbcd-113">Перечисление доступных типов поставщиков</span><span class="sxs-lookup"><span data-stu-id="edbcd-113">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="edbcd-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="edbcd-114">String collection</span></span>|<span data-ttu-id="edbcd-115">Получение всех доступных типов поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="edbcd-115">Retrieve all available identity provider types.</span></span>|

## <a name="properties"></a><span data-ttu-id="edbcd-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="edbcd-116">Properties</span></span>

|<span data-ttu-id="edbcd-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="edbcd-117">Property</span></span>|<span data-ttu-id="edbcd-118">Тип</span><span class="sxs-lookup"><span data-stu-id="edbcd-118">Type</span></span>|<span data-ttu-id="edbcd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="edbcd-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edbcd-120">id</span><span class="sxs-lookup"><span data-stu-id="edbcd-120">id</span></span>|<span data-ttu-id="edbcd-121">String</span><span class="sxs-lookup"><span data-stu-id="edbcd-121">String</span></span>|<span data-ttu-id="edbcd-122">Идентификатор поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="edbcd-122">The ID of the identity provider.</span></span>|
|<span data-ttu-id="edbcd-123">displayName</span><span class="sxs-lookup"><span data-stu-id="edbcd-123">displayName</span></span>|<span data-ttu-id="edbcd-124">String</span><span class="sxs-lookup"><span data-stu-id="edbcd-124">String</span></span>|<span data-ttu-id="edbcd-125">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="edbcd-125">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edbcd-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edbcd-126">JSON representation</span></span>

<span data-ttu-id="edbcd-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edbcd-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
