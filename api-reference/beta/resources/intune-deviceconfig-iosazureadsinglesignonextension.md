---
title: Тип ресурса Иосазуреадсинглесигнонекстенсион
description: Представляет профиль расширения единого входа Azure AD для устройств с iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9388b46457df2390a0820c1005f0df0e1cae9b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444208"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="6130d-103">Тип ресурса Иосазуреадсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="6130d-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="6130d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6130d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6130d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6130d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6130d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6130d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6130d-107">Представляет профиль расширения единого входа Azure AD для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="6130d-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="6130d-108">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="6130d-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6130d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6130d-109">Properties</span></span>
|<span data-ttu-id="6130d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6130d-110">Property</span></span>|<span data-ttu-id="6130d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6130d-111">Type</span></span>|<span data-ttu-id="6130d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6130d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6130d-113">енаблешареддевицемоде</span><span class="sxs-lookup"><span data-stu-id="6130d-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="6130d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6130d-114">Boolean</span></span>|<span data-ttu-id="6130d-115">Включает или отключает режим общего устройства.</span><span class="sxs-lookup"><span data-stu-id="6130d-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="6130d-116">построения</span><span class="sxs-lookup"><span data-stu-id="6130d-116">configurations</span></span>|<span data-ttu-id="6130d-117">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6130d-117">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="6130d-118">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="6130d-118">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="6130d-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6130d-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6130d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6130d-120">Relationships</span></span>
<span data-ttu-id="6130d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6130d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6130d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6130d-122">JSON Representation</span></span>
<span data-ttu-id="6130d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6130d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



