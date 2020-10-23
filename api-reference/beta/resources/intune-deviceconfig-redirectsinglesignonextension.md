---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение Apple Single Sign-On.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b51e708889bd4d6e81f50a326143deef7bd40f4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693915"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="47dfb-103">Тип ресурса Редиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="47dfb-103">redirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="47dfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47dfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47dfb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47dfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47dfb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47dfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47dfb-107">Представляет расширение Apple Single Sign-On.</span><span class="sxs-lookup"><span data-stu-id="47dfb-107">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="47dfb-108">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="47dfb-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47dfb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47dfb-109">Properties</span></span>
|<span data-ttu-id="47dfb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47dfb-110">Property</span></span>|<span data-ttu-id="47dfb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47dfb-111">Type</span></span>|<span data-ttu-id="47dfb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47dfb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47dfb-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="47dfb-113">extensionIdentifier</span></span>|<span data-ttu-id="47dfb-114">Строка</span><span class="sxs-lookup"><span data-stu-id="47dfb-114">String</span></span>|<span data-ttu-id="47dfb-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="47dfb-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="47dfb-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="47dfb-116">teamIdentifier</span></span>|<span data-ttu-id="47dfb-117">Строка</span><span class="sxs-lookup"><span data-stu-id="47dfb-117">String</span></span>|<span data-ttu-id="47dfb-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="47dfb-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="47dfb-119">построения</span><span class="sxs-lookup"><span data-stu-id="47dfb-119">configurations</span></span>|<span data-ttu-id="47dfb-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="47dfb-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="47dfb-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="47dfb-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="47dfb-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="47dfb-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47dfb-123">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="47dfb-123">urlPrefixes</span></span>|<span data-ttu-id="47dfb-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="47dfb-124">String collection</span></span>|<span data-ttu-id="47dfb-125">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="47dfb-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="47dfb-126">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="47dfb-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="47dfb-127">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="47dfb-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47dfb-128">Связи</span><span class="sxs-lookup"><span data-stu-id="47dfb-128">Relationships</span></span>
<span data-ttu-id="47dfb-129">Нет</span><span class="sxs-lookup"><span data-stu-id="47dfb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47dfb-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47dfb-130">JSON Representation</span></span>
<span data-ttu-id="47dfb-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47dfb-131">Here is a JSON representation of the resource.</span></span>
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





