---
title: Тип ресурса adminConsent
description: Сведения о разрешения администратора.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 428729ff9a8a8ee5deb64c537922cb7a0417ba2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962130"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="57ee7-103">Тип ресурса adminConsent</span><span class="sxs-lookup"><span data-stu-id="57ee7-103">adminConsent resource type</span></span>

> <span data-ttu-id="57ee7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57ee7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57ee7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57ee7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="57ee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57ee7-107">Сведения о разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="57ee7-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="57ee7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="57ee7-108">Properties</span></span>
|<span data-ttu-id="57ee7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="57ee7-109">Property</span></span>|<span data-ttu-id="57ee7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="57ee7-110">Type</span></span>|<span data-ttu-id="57ee7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="57ee7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ee7-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="57ee7-112">shareAPNSData</span></span>|[<span data-ttu-id="57ee7-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="57ee7-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="57ee7-114">Состояние разрешения администратора общего доступа пользователей и данных устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="57ee7-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="57ee7-115">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="57ee7-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57ee7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="57ee7-116">Relationships</span></span>
<span data-ttu-id="57ee7-117">Нет</span><span class="sxs-lookup"><span data-stu-id="57ee7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57ee7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57ee7-118">JSON Representation</span></span>
<span data-ttu-id="57ee7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57ee7-119">Here is a JSON representation of the resource.</span></span>
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





