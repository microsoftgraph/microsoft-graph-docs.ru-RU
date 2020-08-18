---
title: Тип ресурса Иосазуреадсинглесигнонекстенсион
description: Представляет профиль расширения единого входа Azure AD для устройств с iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd1eacccc09926c65a8e5faf3c61321b472d2013
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790464"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="c2747-103">Тип ресурса Иосазуреадсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="c2747-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="c2747-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2747-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2747-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2747-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2747-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2747-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2747-107">Представляет профиль расширения единого входа Azure AD для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="c2747-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="c2747-108">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="c2747-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2747-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2747-109">Properties</span></span>
|<span data-ttu-id="c2747-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2747-110">Property</span></span>|<span data-ttu-id="c2747-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2747-111">Type</span></span>|<span data-ttu-id="c2747-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2747-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2747-113">енаблешареддевицемоде</span><span class="sxs-lookup"><span data-stu-id="c2747-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="c2747-114">Логический</span><span class="sxs-lookup"><span data-stu-id="c2747-114">Boolean</span></span>|<span data-ttu-id="c2747-115">Включает или отключает режим общего устройства.</span><span class="sxs-lookup"><span data-stu-id="c2747-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="c2747-116">бундлеидакцессконтроллист</span><span class="sxs-lookup"><span data-stu-id="c2747-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="c2747-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2747-117">String collection</span></span>|<span data-ttu-id="c2747-118">Необязательный список дополнительных идентификаторов пакетов, которые могут использовать расширение AAD для единого входа.</span><span class="sxs-lookup"><span data-stu-id="c2747-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="c2747-119">построения</span><span class="sxs-lookup"><span data-stu-id="c2747-119">configurations</span></span>|<span data-ttu-id="c2747-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c2747-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="c2747-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="c2747-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="c2747-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c2747-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2747-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c2747-123">Relationships</span></span>
<span data-ttu-id="c2747-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c2747-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2747-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2747-125">JSON Representation</span></span>
<span data-ttu-id="c2747-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2747-126">Here is a JSON representation of the resource.</span></span>
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



