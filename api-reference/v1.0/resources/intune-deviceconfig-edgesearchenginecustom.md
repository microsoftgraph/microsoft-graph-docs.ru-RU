---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38308433f5e68d921a98e7b030540c465b33fe44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957937"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="92fc3-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="92fc3-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="92fc3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92fc3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92fc3-105">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="92fc3-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="92fc3-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="92fc3-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92fc3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="92fc3-107">Properties</span></span>
|<span data-ttu-id="92fc3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="92fc3-108">Property</span></span>|<span data-ttu-id="92fc3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="92fc3-109">Type</span></span>|<span data-ttu-id="92fc3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92fc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92fc3-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="92fc3-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="92fc3-112">String</span><span class="sxs-lookup"><span data-stu-id="92fc3-112">String</span></span>|<span data-ttu-id="92fc3-113">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="92fc3-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92fc3-114">Связи</span><span class="sxs-lookup"><span data-stu-id="92fc3-114">Relationships</span></span>
<span data-ttu-id="92fc3-115">Нет</span><span class="sxs-lookup"><span data-stu-id="92fc3-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92fc3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92fc3-116">JSON Representation</span></span>
<span data-ttu-id="92fc3-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92fc3-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



