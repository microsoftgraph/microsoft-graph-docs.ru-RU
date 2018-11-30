---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
ms.openlocfilehash: 5312f53e43921d71e6c338ccb112a851773abc43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077870"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="efd3d-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="efd3d-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="efd3d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="efd3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efd3d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd3d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="efd3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efd3d-107">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="efd3d-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="efd3d-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="efd3d-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efd3d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efd3d-109">Properties</span></span>
|<span data-ttu-id="efd3d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="efd3d-110">Property</span></span>|<span data-ttu-id="efd3d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="efd3d-111">Type</span></span>|<span data-ttu-id="efd3d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="efd3d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd3d-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="efd3d-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="efd3d-114">String</span><span class="sxs-lookup"><span data-stu-id="efd3d-114">String</span></span>|<span data-ttu-id="efd3d-115">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="efd3d-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efd3d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="efd3d-116">Relationships</span></span>
<span data-ttu-id="efd3d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="efd3d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="efd3d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efd3d-118">JSON Representation</span></span>
<span data-ttu-id="efd3d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efd3d-119">Here is a JSON representation of the resource.</span></span>
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





