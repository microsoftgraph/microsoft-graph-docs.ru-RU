---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cffa929a063c77010f005a4e0b3da8fd8b7363d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530602"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="0dfa3-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="0dfa3-103">omaSetting resource type</span></span>

<span data-ttu-id="0dfa3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dfa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dfa3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dfa3-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0dfa3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0dfa3-107">Properties</span></span>
|<span data-ttu-id="0dfa3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0dfa3-108">Property</span></span>|<span data-ttu-id="0dfa3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0dfa3-109">Type</span></span>|<span data-ttu-id="0dfa3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0dfa3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dfa3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0dfa3-111">displayName</span></span>|<span data-ttu-id="0dfa3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0dfa3-112">String</span></span>|<span data-ttu-id="0dfa3-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-113">Display Name.</span></span>|
|<span data-ttu-id="0dfa3-114">description</span><span class="sxs-lookup"><span data-stu-id="0dfa3-114">description</span></span>|<span data-ttu-id="0dfa3-115">String</span><span class="sxs-lookup"><span data-stu-id="0dfa3-115">String</span></span>|<span data-ttu-id="0dfa3-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-116">Description.</span></span>|
|<span data-ttu-id="0dfa3-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0dfa3-117">omaUri</span></span>|<span data-ttu-id="0dfa3-118">String</span><span class="sxs-lookup"><span data-stu-id="0dfa3-118">String</span></span>|<span data-ttu-id="0dfa3-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dfa3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0dfa3-120">Relationships</span></span>
<span data-ttu-id="0dfa3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0dfa3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dfa3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0dfa3-122">JSON Representation</span></span>
<span data-ttu-id="0dfa3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0dfa3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




