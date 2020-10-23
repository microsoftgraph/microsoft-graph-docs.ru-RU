---
title: Тип ресурса Макосазуреадсинглесигнонекстенсион
description: Представляет один Sign-Onный профиль расширения Azure AD для устройств macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bc80bb752230fd1699091c380538e62d4ca09c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736249"
---
# <a name="macosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="7411a-103">Тип ресурса Макосазуреадсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="7411a-103">macOSAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="7411a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7411a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7411a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7411a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7411a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7411a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7411a-107">Представляет один Sign-Onный профиль расширения Azure AD для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="7411a-107">Represents an Azure AD-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="7411a-108">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="7411a-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7411a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7411a-109">Properties</span></span>
|<span data-ttu-id="7411a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7411a-110">Property</span></span>|<span data-ttu-id="7411a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7411a-111">Type</span></span>|<span data-ttu-id="7411a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7411a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7411a-113">енаблешареддевицемоде</span><span class="sxs-lookup"><span data-stu-id="7411a-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="7411a-114">Логический</span><span class="sxs-lookup"><span data-stu-id="7411a-114">Boolean</span></span>|<span data-ttu-id="7411a-115">Включает или отключает режим общего устройства.</span><span class="sxs-lookup"><span data-stu-id="7411a-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="7411a-116">бундлеидакцессконтроллист</span><span class="sxs-lookup"><span data-stu-id="7411a-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="7411a-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7411a-117">String collection</span></span>|<span data-ttu-id="7411a-118">Необязательный список дополнительных идентификаторов пакетов, которые могут использовать расширение AAD для единого входа.</span><span class="sxs-lookup"><span data-stu-id="7411a-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="7411a-119">построения</span><span class="sxs-lookup"><span data-stu-id="7411a-119">configurations</span></span>|<span data-ttu-id="7411a-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7411a-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="7411a-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="7411a-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="7411a-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7411a-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7411a-123">Связи</span><span class="sxs-lookup"><span data-stu-id="7411a-123">Relationships</span></span>
<span data-ttu-id="7411a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="7411a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7411a-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7411a-125">JSON Representation</span></span>
<span data-ttu-id="7411a-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7411a-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```





