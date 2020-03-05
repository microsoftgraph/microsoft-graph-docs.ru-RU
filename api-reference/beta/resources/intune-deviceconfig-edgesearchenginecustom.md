---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f960c68e0ecce4cebdbd4727c77eae971cb5ce70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530037"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="cc2f6-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="cc2f6-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="cc2f6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cc2f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc2f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc2f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc2f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc2f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc2f6-107">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="cc2f6-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="cc2f6-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="cc2f6-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc2f6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc2f6-109">Properties</span></span>
|<span data-ttu-id="cc2f6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc2f6-110">Property</span></span>|<span data-ttu-id="cc2f6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cc2f6-111">Type</span></span>|<span data-ttu-id="cc2f6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2f6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2f6-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="cc2f6-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="cc2f6-114">String</span><span class="sxs-lookup"><span data-stu-id="cc2f6-114">String</span></span>|<span data-ttu-id="cc2f6-115">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="cc2f6-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc2f6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="cc2f6-116">Relationships</span></span>
<span data-ttu-id="cc2f6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="cc2f6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc2f6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc2f6-118">JSON Representation</span></span>
<span data-ttu-id="cc2f6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc2f6-119">Here is a JSON representation of the resource.</span></span>
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



