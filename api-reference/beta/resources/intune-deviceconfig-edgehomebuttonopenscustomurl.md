---
title: Тип ресурса edgeHomeButtonOpensCustomURL
description: Кнопка "Показать Домашняя страница"; Нажатие кнопки Домой загружает определенного URL-адреса.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06f73375772f53b546e7e9b758a7513366949326
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431765"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="d0554-103">Тип ресурса edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="d0554-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="d0554-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0554-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0554-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0554-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0554-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0554-107">Кнопка "Показать Домашняя страница"; Нажатие кнопки Домой загружает определенного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="d0554-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="d0554-108">Наследуется от [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0554-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0554-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0554-109">Properties</span></span>
|<span data-ttu-id="d0554-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0554-110">Property</span></span>|<span data-ttu-id="d0554-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d0554-111">Type</span></span>|<span data-ttu-id="d0554-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0554-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0554-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="d0554-113">homeButtonCustomURL</span></span>|<span data-ttu-id="d0554-114">String</span><span class="sxs-lookup"><span data-stu-id="d0554-114">String</span></span>|<span data-ttu-id="d0554-115">Определенного URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="d0554-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0554-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="d0554-116">Relationships</span></span>
<span data-ttu-id="d0554-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d0554-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0554-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0554-118">JSON Representation</span></span>
<span data-ttu-id="d0554-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0554-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




