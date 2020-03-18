---
title: Тип ресурса Макоскредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ec152f59cba88c2bb3e02e5fc90aba2a8c6f94a2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790302"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="ad289-103">Тип ресурса Макоскредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="ad289-103">macOSCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="ad289-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad289-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad289-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad289-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad289-106">Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="ad289-106">Represents a Credential-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="ad289-107">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="ad289-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad289-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad289-108">Properties</span></span>
|<span data-ttu-id="ad289-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad289-109">Property</span></span>|<span data-ttu-id="ad289-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ad289-110">Type</span></span>|<span data-ttu-id="ad289-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ad289-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad289-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="ad289-112">extensionIdentifier</span></span>|<span data-ttu-id="ad289-113">String</span><span class="sxs-lookup"><span data-stu-id="ad289-113">String</span></span>|<span data-ttu-id="ad289-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ad289-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ad289-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="ad289-115">teamIdentifier</span></span>|<span data-ttu-id="ad289-116">String</span><span class="sxs-lookup"><span data-stu-id="ad289-116">String</span></span>|<span data-ttu-id="ad289-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ad289-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ad289-118">домена</span><span class="sxs-lookup"><span data-stu-id="ad289-118">domains</span></span>|<span data-ttu-id="ad289-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad289-119">String collection</span></span>|<span data-ttu-id="ad289-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="ad289-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="ad289-121">область</span><span class="sxs-lookup"><span data-stu-id="ad289-121">realm</span></span>|<span data-ttu-id="ad289-122">String</span><span class="sxs-lookup"><span data-stu-id="ad289-122">String</span></span>|<span data-ttu-id="ad289-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="ad289-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="ad289-124">построения</span><span class="sxs-lookup"><span data-stu-id="ad289-124">configurations</span></span>|<span data-ttu-id="ad289-125">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ad289-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="ad289-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ad289-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="ad289-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ad289-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad289-128">Связи</span><span class="sxs-lookup"><span data-stu-id="ad289-128">Relationships</span></span>
<span data-ttu-id="ad289-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ad289-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad289-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad289-130">JSON Representation</span></span>
<span data-ttu-id="ad289-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad289-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



