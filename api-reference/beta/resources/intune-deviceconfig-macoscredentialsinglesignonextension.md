---
title: Тип ресурса Макоскредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 226f9bc0ec559bad7ba155aff6da864525882822
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163474"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="f6d90-103">Тип ресурса Макоскредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="f6d90-103">macOSCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="f6d90-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d90-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6d90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d90-106">Представляет профиль расширения единого входа с типом учетных данных для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="f6d90-106">Represents a Credential-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="f6d90-107">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="f6d90-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6d90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6d90-108">Properties</span></span>
|<span data-ttu-id="f6d90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6d90-109">Property</span></span>|<span data-ttu-id="f6d90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f6d90-110">Type</span></span>|<span data-ttu-id="f6d90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f6d90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d90-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="f6d90-112">extensionIdentifier</span></span>|<span data-ttu-id="f6d90-113">String</span><span class="sxs-lookup"><span data-stu-id="f6d90-113">String</span></span>|<span data-ttu-id="f6d90-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6d90-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f6d90-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="f6d90-115">teamIdentifier</span></span>|<span data-ttu-id="f6d90-116">String</span><span class="sxs-lookup"><span data-stu-id="f6d90-116">String</span></span>|<span data-ttu-id="f6d90-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6d90-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f6d90-118">домена</span><span class="sxs-lookup"><span data-stu-id="f6d90-118">domains</span></span>|<span data-ttu-id="f6d90-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f6d90-119">String collection</span></span>|<span data-ttu-id="f6d90-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="f6d90-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="f6d90-121">область</span><span class="sxs-lookup"><span data-stu-id="f6d90-121">realm</span></span>|<span data-ttu-id="f6d90-122">String</span><span class="sxs-lookup"><span data-stu-id="f6d90-122">String</span></span>|<span data-ttu-id="f6d90-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="f6d90-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="f6d90-124">построения</span><span class="sxs-lookup"><span data-stu-id="f6d90-124">configurations</span></span>|<span data-ttu-id="f6d90-125">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f6d90-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="f6d90-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f6d90-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="f6d90-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6d90-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6d90-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="f6d90-128">Relationships</span></span>
<span data-ttu-id="f6d90-129">Нет</span><span class="sxs-lookup"><span data-stu-id="f6d90-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6d90-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6d90-130">JSON Representation</span></span>
<span data-ttu-id="f6d90-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6d90-131">Here is a JSON representation of the resource.</span></span>
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



