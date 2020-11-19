---
title: Тип ресурса Виндовскиосказуреадусер
description: Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03fffb8bf5a2871206b775d4708ac0d5b2c52c22
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293474"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="746c6-103">Тип ресурса Виндовскиосказуреадусер</span><span class="sxs-lookup"><span data-stu-id="746c6-103">windowsKioskAzureADUser resource type</span></span>

<span data-ttu-id="746c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="746c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="746c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="746c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="746c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="746c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="746c6-107">Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="746c6-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="746c6-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="746c6-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="746c6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="746c6-109">Properties</span></span>
|<span data-ttu-id="746c6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="746c6-110">Property</span></span>|<span data-ttu-id="746c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="746c6-111">Type</span></span>|<span data-ttu-id="746c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="746c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="746c6-113">userId</span><span class="sxs-lookup"><span data-stu-id="746c6-113">userId</span></span>|<span data-ttu-id="746c6-114">String</span><span class="sxs-lookup"><span data-stu-id="746c6-114">String</span></span>|<span data-ttu-id="746c6-115">Идентификатор пользователя AzureAD, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="746c6-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="746c6-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="746c6-116">userPrincipalName</span></span>|<span data-ttu-id="746c6-117">String</span><span class="sxs-lookup"><span data-stu-id="746c6-117">String</span></span>|<span data-ttu-id="746c6-118">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="746c6-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="746c6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="746c6-119">Relationships</span></span>
<span data-ttu-id="746c6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="746c6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="746c6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="746c6-121">JSON Representation</span></span>
<span data-ttu-id="746c6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="746c6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




