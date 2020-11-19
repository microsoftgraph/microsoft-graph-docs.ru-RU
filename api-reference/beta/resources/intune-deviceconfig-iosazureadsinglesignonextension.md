---
title: Тип ресурса Иосазуреадсинглесигнонекстенсион
description: Представляет один Sign-Onный профиль расширения Azure AD для устройств с iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12bfdea3ee6c5b07d8a94f82d4344b2d679f627e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280566"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="42288-103">Тип ресурса Иосазуреадсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="42288-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="42288-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42288-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42288-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42288-107">Представляет один Sign-Onный профиль расширения Azure AD для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="42288-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="42288-108">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="42288-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42288-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="42288-109">Properties</span></span>
|<span data-ttu-id="42288-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="42288-110">Property</span></span>|<span data-ttu-id="42288-111">Тип</span><span class="sxs-lookup"><span data-stu-id="42288-111">Type</span></span>|<span data-ttu-id="42288-112">Описание</span><span class="sxs-lookup"><span data-stu-id="42288-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42288-113">енаблешареддевицемоде</span><span class="sxs-lookup"><span data-stu-id="42288-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="42288-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="42288-114">Boolean</span></span>|<span data-ttu-id="42288-115">Включает или отключает режим общего устройства.</span><span class="sxs-lookup"><span data-stu-id="42288-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="42288-116">бундлеидакцессконтроллист</span><span class="sxs-lookup"><span data-stu-id="42288-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="42288-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42288-117">String collection</span></span>|<span data-ttu-id="42288-118">Необязательный список дополнительных идентификаторов пакетов, которые могут использовать расширение AAD для единого входа.</span><span class="sxs-lookup"><span data-stu-id="42288-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="42288-119">построения</span><span class="sxs-lookup"><span data-stu-id="42288-119">configurations</span></span>|<span data-ttu-id="42288-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="42288-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="42288-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="42288-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="42288-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="42288-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42288-123">Связи</span><span class="sxs-lookup"><span data-stu-id="42288-123">Relationships</span></span>
<span data-ttu-id="42288-124">Нет</span><span class="sxs-lookup"><span data-stu-id="42288-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42288-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42288-125">JSON Representation</span></span>
<span data-ttu-id="42288-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42288-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```




