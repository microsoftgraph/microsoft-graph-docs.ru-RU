---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение Apple Single Sign-On.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b899a0bfcb80c57bdfc889a4a857950678946c6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198222"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="4bef2-103">Тип ресурса Редиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="4bef2-103">redirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="4bef2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bef2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bef2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bef2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bef2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bef2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bef2-107">Представляет расширение Apple Single Sign-On.</span><span class="sxs-lookup"><span data-stu-id="4bef2-107">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="4bef2-108">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="4bef2-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4bef2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bef2-109">Properties</span></span>
|<span data-ttu-id="4bef2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bef2-110">Property</span></span>|<span data-ttu-id="4bef2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4bef2-111">Type</span></span>|<span data-ttu-id="4bef2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4bef2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bef2-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="4bef2-113">extensionIdentifier</span></span>|<span data-ttu-id="4bef2-114">String</span><span class="sxs-lookup"><span data-stu-id="4bef2-114">String</span></span>|<span data-ttu-id="4bef2-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4bef2-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4bef2-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="4bef2-116">teamIdentifier</span></span>|<span data-ttu-id="4bef2-117">String</span><span class="sxs-lookup"><span data-stu-id="4bef2-117">String</span></span>|<span data-ttu-id="4bef2-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4bef2-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4bef2-119">построения</span><span class="sxs-lookup"><span data-stu-id="4bef2-119">configurations</span></span>|<span data-ttu-id="4bef2-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4bef2-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="4bef2-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4bef2-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="4bef2-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4bef2-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4bef2-123">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="4bef2-123">urlPrefixes</span></span>|<span data-ttu-id="4bef2-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4bef2-124">String collection</span></span>|<span data-ttu-id="4bef2-125">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="4bef2-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="4bef2-126">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="4bef2-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="4bef2-127">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="4bef2-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bef2-128">Связи</span><span class="sxs-lookup"><span data-stu-id="4bef2-128">Relationships</span></span>
<span data-ttu-id="4bef2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4bef2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bef2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bef2-130">JSON Representation</span></span>
<span data-ttu-id="4bef2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bef2-131">Here is a JSON representation of the resource.</span></span>
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




