---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cd8f4ad66a80873d24f6ed14785e1f24d88077c4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467481"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="95ead-103">тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="95ead-103">configuration resource type</span></span>

<span data-ttu-id="95ead-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="95ead-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="95ead-105">Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="95ead-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="95ead-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="95ead-106">Properties</span></span>
|<span data-ttu-id="95ead-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="95ead-107">Property</span></span>|<span data-ttu-id="95ead-108">Тип</span><span class="sxs-lookup"><span data-stu-id="95ead-108">Type</span></span>|<span data-ttu-id="95ead-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95ead-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ead-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="95ead-110">authorizedAppIds</span></span>|<span data-ttu-id="95ead-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95ead-111">String collection</span></span>|<span data-ttu-id="95ead-112">Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.</span><span class="sxs-lookup"><span data-stu-id="95ead-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95ead-113">Связи</span><span class="sxs-lookup"><span data-stu-id="95ead-113">Relationships</span></span>
<span data-ttu-id="95ead-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="95ead-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95ead-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95ead-115">JSON representation</span></span>
<span data-ttu-id="95ead-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95ead-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

