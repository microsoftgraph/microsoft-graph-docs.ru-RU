---
title: Тип ресурса windowsKioskActiveDirectoryGroup
description: Класс, используемый для идентификации группу Azure Directory для базовой конфигурации
ms.openlocfilehash: 18e876b50bdc8c8946bd511348d6ed3a6fc8fe5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076593"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="54037-103">Тип ресурса windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="54037-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="54037-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54037-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54037-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54037-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54037-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54037-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54037-107">Класс, используемый для идентификации группу Azure Directory для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="54037-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="54037-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="54037-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54037-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="54037-109">Properties</span></span>
|<span data-ttu-id="54037-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="54037-110">Property</span></span>|<span data-ttu-id="54037-111">Тип</span><span class="sxs-lookup"><span data-stu-id="54037-111">Type</span></span>|<span data-ttu-id="54037-112">Description</span><span class="sxs-lookup"><span data-stu-id="54037-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54037-113">groupName</span><span class="sxs-lookup"><span data-stu-id="54037-113">groupName</span></span>|<span data-ttu-id="54037-114">String</span><span class="sxs-lookup"><span data-stu-id="54037-114">String</span></span>|<span data-ttu-id="54037-115">Имя группы AD, которая будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="54037-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="54037-116">Связи</span><span class="sxs-lookup"><span data-stu-id="54037-116">Relationships</span></span>
<span data-ttu-id="54037-117">Нет</span><span class="sxs-lookup"><span data-stu-id="54037-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54037-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54037-118">JSON Representation</span></span>
<span data-ttu-id="54037-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54037-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





