---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации службы каталогов для контактных сущностями пользователя, группы или организации при синхронизации локального каталога с Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: japere
ms.openlocfilehash: e4e3469ae371568ac9010d1d3879f68c92340460
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133982"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="0eabc-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="0eabc-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="0eabc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eabc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eabc-105">Представляет ошибки синхронизации службы каталогов для [](orgcontact.md) пользовательских, [](user.md)групповых или организационных контактных сущностями при синхронизации локального каталога с Azure Active Directory. [](group.md)</span><span class="sxs-lookup"><span data-stu-id="0eabc-105">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="0eabc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0eabc-106">Properties</span></span>

| <span data-ttu-id="0eabc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eabc-107">Property</span></span> | <span data-ttu-id="0eabc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0eabc-108">Type</span></span> | <span data-ttu-id="0eabc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0eabc-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0eabc-110">category</span><span class="sxs-lookup"><span data-stu-id="0eabc-110">category</span></span>|<span data-ttu-id="0eabc-111">String</span><span class="sxs-lookup"><span data-stu-id="0eabc-111">String</span></span>| <span data-ttu-id="0eabc-112">Категория ошибки при предоставлении.</span><span class="sxs-lookup"><span data-stu-id="0eabc-112">Category of the provisioning error.</span></span> <span data-ttu-id="0eabc-113">Примечание. В настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="0eabc-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="0eabc-114">Возможное *значение: PropertyConflict* — указывает, что значение свойства не уникально.</span><span class="sxs-lookup"><span data-stu-id="0eabc-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="0eabc-115">Другие объекты содержат такое же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="0eabc-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="0eabc-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="0eabc-116">occurredDateTime</span></span>|<span data-ttu-id="0eabc-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eabc-117">DateTimeOffset</span></span>| <span data-ttu-id="0eabc-118">Дата и время, когда произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="0eabc-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="0eabc-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="0eabc-119">propertyCausingError</span></span>|<span data-ttu-id="0eabc-120">Строка</span><span class="sxs-lookup"><span data-stu-id="0eabc-120">String</span></span>| <span data-ttu-id="0eabc-121">Имя свойства каталога, вызываемого ошибкой.</span><span class="sxs-lookup"><span data-stu-id="0eabc-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="0eabc-122">Текущие возможные значения: *UserPrincipalName или* *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="0eabc-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="0eabc-123">value</span><span class="sxs-lookup"><span data-stu-id="0eabc-123">value</span></span>|<span data-ttu-id="0eabc-124">String</span><span class="sxs-lookup"><span data-stu-id="0eabc-124">String</span></span>| <span data-ttu-id="0eabc-125">Значение свойства, вызываемого ошибкой.</span><span class="sxs-lookup"><span data-stu-id="0eabc-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0eabc-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0eabc-126">JSON representation</span></span>
<span data-ttu-id="0eabc-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eabc-127">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


