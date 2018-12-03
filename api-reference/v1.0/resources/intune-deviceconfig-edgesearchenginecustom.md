---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
ms.openlocfilehash: 54617b01fc3082fc8c80b653e7df36e48c1de0d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026220"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="afe3f-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="afe3f-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="afe3f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afe3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afe3f-105">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="afe3f-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="afe3f-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="afe3f-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afe3f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="afe3f-107">Properties</span></span>
|<span data-ttu-id="afe3f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="afe3f-108">Property</span></span>|<span data-ttu-id="afe3f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="afe3f-109">Type</span></span>|<span data-ttu-id="afe3f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="afe3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afe3f-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="afe3f-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="afe3f-112">String</span><span class="sxs-lookup"><span data-stu-id="afe3f-112">String</span></span>|<span data-ttu-id="afe3f-113">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="afe3f-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afe3f-114">Связи</span><span class="sxs-lookup"><span data-stu-id="afe3f-114">Relationships</span></span>
<span data-ttu-id="afe3f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="afe3f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afe3f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afe3f-116">JSON Representation</span></span>
<span data-ttu-id="afe3f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afe3f-117">Here is a JSON representation of the resource.</span></span>
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



