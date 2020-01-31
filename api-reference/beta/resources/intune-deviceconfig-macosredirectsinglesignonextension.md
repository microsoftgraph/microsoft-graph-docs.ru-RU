---
title: Тип ресурса Макосредиректсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с перенаправлением для устройств macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba8f2aacd8ffd02a7c0c48274e5da5a4bc22addb
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636304"
---
# <a name="macosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="4000b-103">Тип ресурса Макосредиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="4000b-103">macOSRedirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="4000b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4000b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4000b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4000b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4000b-106">Представляет профиль расширения единого входа с перенаправлением для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="4000b-106">Represents a Redirect-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="4000b-107">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="4000b-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4000b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4000b-108">Properties</span></span>
|<span data-ttu-id="4000b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4000b-109">Property</span></span>|<span data-ttu-id="4000b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4000b-110">Type</span></span>|<span data-ttu-id="4000b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4000b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4000b-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="4000b-112">extensionIdentifier</span></span>|<span data-ttu-id="4000b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4000b-113">String</span></span>|<span data-ttu-id="4000b-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4000b-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4000b-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="4000b-115">teamIdentifier</span></span>|<span data-ttu-id="4000b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="4000b-116">String</span></span>|<span data-ttu-id="4000b-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4000b-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4000b-118">построения</span><span class="sxs-lookup"><span data-stu-id="4000b-118">configurations</span></span>|<span data-ttu-id="4000b-119">Коллекция [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4000b-119">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="4000b-120">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4000b-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="4000b-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4000b-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4000b-122">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="4000b-122">urlPrefixes</span></span>|<span data-ttu-id="4000b-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4000b-123">String collection</span></span>|<span data-ttu-id="4000b-124">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="4000b-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="4000b-125">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="4000b-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="4000b-126">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="4000b-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4000b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="4000b-127">Relationships</span></span>
<span data-ttu-id="4000b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="4000b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4000b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4000b-129">JSON Representation</span></span>
<span data-ttu-id="4000b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4000b-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



