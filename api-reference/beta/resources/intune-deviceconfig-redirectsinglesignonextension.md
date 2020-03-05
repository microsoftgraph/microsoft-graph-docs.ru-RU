---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение единого входа Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8398bcc1f10c91750b71928472290ccde55dad23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529462"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="9421d-103">Тип ресурса Редиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="9421d-103">redirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="9421d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9421d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9421d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9421d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9421d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9421d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9421d-107">Представляет расширение единого входа Apple.</span><span class="sxs-lookup"><span data-stu-id="9421d-107">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="9421d-108">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="9421d-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9421d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9421d-109">Properties</span></span>
|<span data-ttu-id="9421d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9421d-110">Property</span></span>|<span data-ttu-id="9421d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9421d-111">Type</span></span>|<span data-ttu-id="9421d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9421d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9421d-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="9421d-113">extensionIdentifier</span></span>|<span data-ttu-id="9421d-114">String</span><span class="sxs-lookup"><span data-stu-id="9421d-114">String</span></span>|<span data-ttu-id="9421d-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="9421d-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="9421d-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="9421d-116">teamIdentifier</span></span>|<span data-ttu-id="9421d-117">String</span><span class="sxs-lookup"><span data-stu-id="9421d-117">String</span></span>|<span data-ttu-id="9421d-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="9421d-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="9421d-119">построения</span><span class="sxs-lookup"><span data-stu-id="9421d-119">configurations</span></span>|<span data-ttu-id="9421d-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9421d-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="9421d-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="9421d-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="9421d-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9421d-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9421d-123">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="9421d-123">urlPrefixes</span></span>|<span data-ttu-id="9421d-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9421d-124">String collection</span></span>|<span data-ttu-id="9421d-125">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="9421d-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="9421d-126">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="9421d-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="9421d-127">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="9421d-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9421d-128">Связи</span><span class="sxs-lookup"><span data-stu-id="9421d-128">Relationships</span></span>
<span data-ttu-id="9421d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="9421d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9421d-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9421d-130">JSON Representation</span></span>
<span data-ttu-id="9421d-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9421d-131">Here is a JSON representation of the resource.</span></span>
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



