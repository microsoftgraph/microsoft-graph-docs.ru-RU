---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 34137caf93bcdd3a3621842b9976e964b8f44c78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759996"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d347a-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="d347a-103">omaSetting resource type</span></span>

<span data-ttu-id="d347a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d347a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d347a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d347a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d347a-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d347a-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d347a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d347a-107">Properties</span></span>
|<span data-ttu-id="d347a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d347a-108">Property</span></span>|<span data-ttu-id="d347a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d347a-109">Type</span></span>|<span data-ttu-id="d347a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d347a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d347a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d347a-111">displayName</span></span>|<span data-ttu-id="d347a-112">String</span><span class="sxs-lookup"><span data-stu-id="d347a-112">String</span></span>|<span data-ttu-id="d347a-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d347a-113">Display Name.</span></span>|
|<span data-ttu-id="d347a-114">description</span><span class="sxs-lookup"><span data-stu-id="d347a-114">description</span></span>|<span data-ttu-id="d347a-115">String</span><span class="sxs-lookup"><span data-stu-id="d347a-115">String</span></span>|<span data-ttu-id="d347a-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="d347a-116">Description.</span></span>|
|<span data-ttu-id="d347a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="d347a-117">omaUri</span></span>|<span data-ttu-id="d347a-118">String</span><span class="sxs-lookup"><span data-stu-id="d347a-118">String</span></span>|<span data-ttu-id="d347a-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="d347a-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d347a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d347a-120">Relationships</span></span>
<span data-ttu-id="d347a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d347a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d347a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d347a-122">JSON Representation</span></span>
<span data-ttu-id="d347a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d347a-123">Here is a JSON representation of the resource.</span></span>
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




