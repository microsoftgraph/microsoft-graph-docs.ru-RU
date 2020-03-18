---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение единого входа Apple.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9e2acb6e884b0ba64419e6997e9a8fbfd94024b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787630"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="f35d1-103">Тип ресурса Редиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="f35d1-103">redirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="f35d1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f35d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f35d1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f35d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f35d1-106">Представляет расширение единого входа Apple.</span><span class="sxs-lookup"><span data-stu-id="f35d1-106">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="f35d1-107">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="f35d1-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f35d1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f35d1-108">Properties</span></span>
|<span data-ttu-id="f35d1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f35d1-109">Property</span></span>|<span data-ttu-id="f35d1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f35d1-110">Type</span></span>|<span data-ttu-id="f35d1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f35d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f35d1-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="f35d1-112">extensionIdentifier</span></span>|<span data-ttu-id="f35d1-113">String</span><span class="sxs-lookup"><span data-stu-id="f35d1-113">String</span></span>|<span data-ttu-id="f35d1-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f35d1-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f35d1-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="f35d1-115">teamIdentifier</span></span>|<span data-ttu-id="f35d1-116">String</span><span class="sxs-lookup"><span data-stu-id="f35d1-116">String</span></span>|<span data-ttu-id="f35d1-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f35d1-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f35d1-118">построения</span><span class="sxs-lookup"><span data-stu-id="f35d1-118">configurations</span></span>|<span data-ttu-id="f35d1-119">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f35d1-119">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="f35d1-120">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f35d1-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="f35d1-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f35d1-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f35d1-122">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="f35d1-122">urlPrefixes</span></span>|<span data-ttu-id="f35d1-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f35d1-123">String collection</span></span>|<span data-ttu-id="f35d1-124">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="f35d1-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="f35d1-125">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="f35d1-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="f35d1-126">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="f35d1-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f35d1-127">Связи</span><span class="sxs-lookup"><span data-stu-id="f35d1-127">Relationships</span></span>
<span data-ttu-id="f35d1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="f35d1-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f35d1-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f35d1-129">JSON Representation</span></span>
<span data-ttu-id="f35d1-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f35d1-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.redirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.redirectSingleSignOnExtension",
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



