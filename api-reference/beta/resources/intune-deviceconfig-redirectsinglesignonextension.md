---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение единого входа Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d789df2973d673df32dc66e60ca60d085b8b2ae
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163796"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="891b9-103">Тип ресурса Редиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="891b9-103">redirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="891b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="891b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891b9-106">Представляет расширение единого входа Apple.</span><span class="sxs-lookup"><span data-stu-id="891b9-106">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="891b9-107">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="891b9-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="891b9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="891b9-108">Properties</span></span>
|<span data-ttu-id="891b9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="891b9-109">Property</span></span>|<span data-ttu-id="891b9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="891b9-110">Type</span></span>|<span data-ttu-id="891b9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="891b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891b9-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="891b9-112">extensionIdentifier</span></span>|<span data-ttu-id="891b9-113">String</span><span class="sxs-lookup"><span data-stu-id="891b9-113">String</span></span>|<span data-ttu-id="891b9-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="891b9-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="891b9-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="891b9-115">teamIdentifier</span></span>|<span data-ttu-id="891b9-116">String</span><span class="sxs-lookup"><span data-stu-id="891b9-116">String</span></span>|<span data-ttu-id="891b9-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="891b9-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="891b9-118">построения</span><span class="sxs-lookup"><span data-stu-id="891b9-118">configurations</span></span>|<span data-ttu-id="891b9-119">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="891b9-119">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="891b9-120">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="891b9-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="891b9-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="891b9-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="891b9-122">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="891b9-122">urlPrefixes</span></span>|<span data-ttu-id="891b9-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="891b9-123">String collection</span></span>|<span data-ttu-id="891b9-124">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="891b9-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="891b9-125">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="891b9-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="891b9-126">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="891b9-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="891b9-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="891b9-127">Relationships</span></span>
<span data-ttu-id="891b9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="891b9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="891b9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="891b9-129">JSON Representation</span></span>
<span data-ttu-id="891b9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="891b9-130">Here is a JSON representation of the resource.</span></span>
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



