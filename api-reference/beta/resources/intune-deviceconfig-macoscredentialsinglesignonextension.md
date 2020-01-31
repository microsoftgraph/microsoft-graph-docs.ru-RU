---
title: Тип ресурса Макоскредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b57ad16d3c94f50ba27a7e45c3c57e770a3164d
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636681"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="fbf65-103">Тип ресурса Макоскредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="fbf65-103">macOSCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="fbf65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf65-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbf65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf65-106">Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="fbf65-106">Represents a Credential-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="fbf65-107">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="fbf65-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbf65-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbf65-108">Properties</span></span>
|<span data-ttu-id="fbf65-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbf65-109">Property</span></span>|<span data-ttu-id="fbf65-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fbf65-110">Type</span></span>|<span data-ttu-id="fbf65-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fbf65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf65-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="fbf65-112">extensionIdentifier</span></span>|<span data-ttu-id="fbf65-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fbf65-113">String</span></span>|<span data-ttu-id="fbf65-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="fbf65-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="fbf65-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="fbf65-115">teamIdentifier</span></span>|<span data-ttu-id="fbf65-116">Строка</span><span class="sxs-lookup"><span data-stu-id="fbf65-116">String</span></span>|<span data-ttu-id="fbf65-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="fbf65-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="fbf65-118">домена</span><span class="sxs-lookup"><span data-stu-id="fbf65-118">domains</span></span>|<span data-ttu-id="fbf65-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fbf65-119">String collection</span></span>|<span data-ttu-id="fbf65-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="fbf65-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="fbf65-121">область</span><span class="sxs-lookup"><span data-stu-id="fbf65-121">realm</span></span>|<span data-ttu-id="fbf65-122">Строка</span><span class="sxs-lookup"><span data-stu-id="fbf65-122">String</span></span>|<span data-ttu-id="fbf65-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="fbf65-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="fbf65-124">построения</span><span class="sxs-lookup"><span data-stu-id="fbf65-124">configurations</span></span>|<span data-ttu-id="fbf65-125">Коллекция [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fbf65-125">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="fbf65-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="fbf65-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="fbf65-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fbf65-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbf65-128">Связи</span><span class="sxs-lookup"><span data-stu-id="fbf65-128">Relationships</span></span>
<span data-ttu-id="fbf65-129">Нет</span><span class="sxs-lookup"><span data-stu-id="fbf65-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbf65-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbf65-130">JSON Representation</span></span>
<span data-ttu-id="fbf65-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbf65-131">Here is a JSON representation of the resource.</span></span>
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



