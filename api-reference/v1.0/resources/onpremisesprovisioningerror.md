---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719bb525fad934bb92f44fb427d1214bf288ec46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059091"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="12c4d-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="12c4d-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="12c4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12c4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12c4d-105">Представляет ошибки синхронизации каталогов для [пользователей](user.md), [групп](group.md) и [orgContact](orgcontact.md) ресурсов при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12c4d-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="12c4d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="12c4d-106">Properties</span></span>

| <span data-ttu-id="12c4d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="12c4d-107">Property</span></span> | <span data-ttu-id="12c4d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="12c4d-108">Type</span></span> | <span data-ttu-id="12c4d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12c4d-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="12c4d-110">category</span><span class="sxs-lookup"><span data-stu-id="12c4d-110">category</span></span>|<span data-ttu-id="12c4d-111">String</span><span class="sxs-lookup"><span data-stu-id="12c4d-111">String</span></span>| <span data-ttu-id="12c4d-112">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="12c4d-112">Category of the provisioning error.</span></span> <span data-ttu-id="12c4d-113">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="12c4d-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="12c4d-114">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="12c4d-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="12c4d-115">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="12c4d-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="12c4d-116">оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="12c4d-116">occurredDateTime</span></span>|<span data-ttu-id="12c4d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c4d-117">DateTimeOffset</span></span>| <span data-ttu-id="12c4d-118">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="12c4d-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="12c4d-119">пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="12c4d-119">propertyCausingError</span></span>|<span data-ttu-id="12c4d-120">String</span><span class="sxs-lookup"><span data-stu-id="12c4d-120">String</span></span>| <span data-ttu-id="12c4d-121">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="12c4d-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="12c4d-122">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="12c4d-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="12c4d-123">value</span><span class="sxs-lookup"><span data-stu-id="12c4d-123">value</span></span>|<span data-ttu-id="12c4d-124">String</span><span class="sxs-lookup"><span data-stu-id="12c4d-124">String</span></span>| <span data-ttu-id="12c4d-125">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="12c4d-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="12c4d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12c4d-126">JSON representation</span></span>
<span data-ttu-id="12c4d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12c4d-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

