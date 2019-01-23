---
title: Тип ресурса adminConsent
description: Сведения о разрешения администратора.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c76ac169bb15792afec908f62b9740e81a4d7e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415882"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="02f44-103">Тип ресурса adminConsent</span><span class="sxs-lookup"><span data-stu-id="02f44-103">adminConsent resource type</span></span>

> <span data-ttu-id="02f44-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02f44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="02f44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02f44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02f44-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02f44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02f44-107">Сведения о разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="02f44-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="02f44-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="02f44-108">Properties</span></span>
|<span data-ttu-id="02f44-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="02f44-109">Property</span></span>|<span data-ttu-id="02f44-110">Тип</span><span class="sxs-lookup"><span data-stu-id="02f44-110">Type</span></span>|<span data-ttu-id="02f44-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02f44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02f44-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="02f44-112">shareAPNSData</span></span>|[<span data-ttu-id="02f44-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="02f44-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="02f44-114">Состояние разрешения администратора общего доступа пользователей и данных устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="02f44-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="02f44-115">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="02f44-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02f44-116">Связи</span><span class="sxs-lookup"><span data-stu-id="02f44-116">Relationships</span></span>
<span data-ttu-id="02f44-117">Нет</span><span class="sxs-lookup"><span data-stu-id="02f44-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02f44-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02f44-118">JSON Representation</span></span>
<span data-ttu-id="02f44-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02f44-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




