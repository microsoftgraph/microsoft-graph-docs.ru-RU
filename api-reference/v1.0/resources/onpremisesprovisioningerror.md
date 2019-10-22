---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccbb10bdf5dba14a01a572198dbdbbafb2534eb7
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621654"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="37742-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="37742-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="37742-104">Представляет ошибки синхронизации каталогов для [пользователей](user.md), [групп](group.md) и [orgContact](orgcontact.md) ресурсов при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="37742-104">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="37742-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="37742-105">Properties</span></span>

| <span data-ttu-id="37742-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="37742-106">Property</span></span> | <span data-ttu-id="37742-107">Тип</span><span class="sxs-lookup"><span data-stu-id="37742-107">Type</span></span> | <span data-ttu-id="37742-108">Описание</span><span class="sxs-lookup"><span data-stu-id="37742-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="37742-109">category</span><span class="sxs-lookup"><span data-stu-id="37742-109">category</span></span>|<span data-ttu-id="37742-110">String</span><span class="sxs-lookup"><span data-stu-id="37742-110">String</span></span>| <span data-ttu-id="37742-111">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="37742-111">Category of the provisioning error.</span></span> <span data-ttu-id="37742-112">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="37742-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="37742-113">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="37742-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="37742-114">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="37742-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="37742-115">оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="37742-115">occurredDateTime</span></span>|<span data-ttu-id="37742-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37742-116">DateTimeOffset</span></span>| <span data-ttu-id="37742-117">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="37742-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="37742-118">пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="37742-118">propertyCausingError</span></span>|<span data-ttu-id="37742-119">String</span><span class="sxs-lookup"><span data-stu-id="37742-119">String</span></span>| <span data-ttu-id="37742-120">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="37742-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="37742-121">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="37742-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="37742-122">value</span><span class="sxs-lookup"><span data-stu-id="37742-122">value</span></span>|<span data-ttu-id="37742-123">String</span><span class="sxs-lookup"><span data-stu-id="37742-123">String</span></span>| <span data-ttu-id="37742-124">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="37742-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37742-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37742-125">JSON representation</span></span>
<span data-ttu-id="37742-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37742-126">Here is a JSON representation of the resource.</span></span>

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
