---
title: Тип ресурса Кредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с типом учетных данных.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72144dc9194f0452b947e2cb72e934893f1721e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795661"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="cd066-103">Тип ресурса Кредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="cd066-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="cd066-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd066-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd066-106">Представляет профиль расширения единого входа с типом учетных данных.</span><span class="sxs-lookup"><span data-stu-id="cd066-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="cd066-107">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="cd066-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cd066-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd066-108">Properties</span></span>
|<span data-ttu-id="cd066-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd066-109">Property</span></span>|<span data-ttu-id="cd066-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cd066-110">Type</span></span>|<span data-ttu-id="cd066-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cd066-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd066-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="cd066-112">extensionIdentifier</span></span>|<span data-ttu-id="cd066-113">String</span><span class="sxs-lookup"><span data-stu-id="cd066-113">String</span></span>|<span data-ttu-id="cd066-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd066-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="cd066-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="cd066-115">teamIdentifier</span></span>|<span data-ttu-id="cd066-116">String</span><span class="sxs-lookup"><span data-stu-id="cd066-116">String</span></span>|<span data-ttu-id="cd066-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd066-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="cd066-118">домена</span><span class="sxs-lookup"><span data-stu-id="cd066-118">domains</span></span>|<span data-ttu-id="cd066-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd066-119">String collection</span></span>|<span data-ttu-id="cd066-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="cd066-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="cd066-121">область</span><span class="sxs-lookup"><span data-stu-id="cd066-121">realm</span></span>|<span data-ttu-id="cd066-122">String</span><span class="sxs-lookup"><span data-stu-id="cd066-122">String</span></span>|<span data-ttu-id="cd066-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="cd066-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="cd066-124">построения</span><span class="sxs-lookup"><span data-stu-id="cd066-124">configurations</span></span>|<span data-ttu-id="cd066-125">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="cd066-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="cd066-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="cd066-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="cd066-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cd066-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd066-128">Связи</span><span class="sxs-lookup"><span data-stu-id="cd066-128">Relationships</span></span>
<span data-ttu-id="cd066-129">Нет</span><span class="sxs-lookup"><span data-stu-id="cd066-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd066-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd066-130">JSON Representation</span></span>
<span data-ttu-id="cd066-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd066-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
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



