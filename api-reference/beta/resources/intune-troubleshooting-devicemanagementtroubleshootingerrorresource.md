---
title: Тип ресурса deviceManagementTroubleshootingErrorResource
description: Объект, представляющий ссылку на ссылку сведения по устранению неполадок может быть на портале Azure или Microsoft doc.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430870"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="bf9ae-103">Тип ресурса deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="bf9ae-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="bf9ae-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf9ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf9ae-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf9ae-107">Объект, представляющий ссылку на ссылку сведения по устранению неполадок может быть на портале Azure или Microsoft doc.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="bf9ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf9ae-108">Properties</span></span>
|<span data-ttu-id="bf9ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf9ae-109">Property</span></span>|<span data-ttu-id="bf9ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bf9ae-110">Type</span></span>|<span data-ttu-id="bf9ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf9ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf9ae-112">text</span><span class="sxs-lookup"><span data-stu-id="bf9ae-112">text</span></span>|<span data-ttu-id="bf9ae-113">String</span><span class="sxs-lookup"><span data-stu-id="bf9ae-113">String</span></span>|<span data-ttu-id="bf9ae-114">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bf9ae-114">Not yet documented</span></span>|
|<span data-ttu-id="bf9ae-115">ссылка</span><span class="sxs-lookup"><span data-stu-id="bf9ae-115">link</span></span>|<span data-ttu-id="bf9ae-116">String</span><span class="sxs-lookup"><span data-stu-id="bf9ae-116">String</span></span>|<span data-ttu-id="bf9ae-117">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-117">The link to the web resource.</span></span> <span data-ttu-id="bf9ae-118">Может содержать любые из следующих форматирования данных: {{имени участника-пользователя}}, {{DeviceGUID}}, {{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="bf9ae-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf9ae-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="bf9ae-119">Relationships</span></span>
<span data-ttu-id="bf9ae-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bf9ae-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf9ae-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf9ae-121">JSON Representation</span></span>
<span data-ttu-id="bf9ae-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf9ae-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




