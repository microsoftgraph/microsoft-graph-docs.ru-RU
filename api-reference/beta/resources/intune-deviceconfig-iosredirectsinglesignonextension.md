---
title: Тип ресурса Иосредиректсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с перенаправлением для устройств с iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0bcff1697c8d41889736cbe74039f8c43d53d680
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790561"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="faa21-103">Тип ресурса Иосредиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="faa21-103">iosRedirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="faa21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faa21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa21-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faa21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa21-106">Представляет профиль расширения единого входа с перенаправлением для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="faa21-106">Represents a Redirect-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="faa21-107">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="faa21-107">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="faa21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="faa21-108">Properties</span></span>
|<span data-ttu-id="faa21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="faa21-109">Property</span></span>|<span data-ttu-id="faa21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="faa21-110">Type</span></span>|<span data-ttu-id="faa21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="faa21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa21-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="faa21-112">extensionIdentifier</span></span>|<span data-ttu-id="faa21-113">String</span><span class="sxs-lookup"><span data-stu-id="faa21-113">String</span></span>|<span data-ttu-id="faa21-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="faa21-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="faa21-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="faa21-115">teamIdentifier</span></span>|<span data-ttu-id="faa21-116">String</span><span class="sxs-lookup"><span data-stu-id="faa21-116">String</span></span>|<span data-ttu-id="faa21-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="faa21-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="faa21-118">построения</span><span class="sxs-lookup"><span data-stu-id="faa21-118">configurations</span></span>|<span data-ttu-id="faa21-119">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="faa21-119">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="faa21-120">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="faa21-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="faa21-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="faa21-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="faa21-122">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="faa21-122">urlPrefixes</span></span>|<span data-ttu-id="faa21-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="faa21-123">String collection</span></span>|<span data-ttu-id="faa21-124">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="faa21-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="faa21-125">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="faa21-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="faa21-126">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="faa21-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa21-127">Связи</span><span class="sxs-lookup"><span data-stu-id="faa21-127">Relationships</span></span>
<span data-ttu-id="faa21-128">Нет</span><span class="sxs-lookup"><span data-stu-id="faa21-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa21-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="faa21-129">JSON Representation</span></span>
<span data-ttu-id="faa21-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faa21-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
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



