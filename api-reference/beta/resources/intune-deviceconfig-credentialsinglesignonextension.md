---
title: Тип ресурса Кредентиалсинглесигнонекстенсион
description: Представляет один профиль расширения Sign-On для типа учетных данных.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 200853c00dfd062d60b337dd9500b38c81774159
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729814"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="9818c-103">Тип ресурса Кредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="9818c-103">credentialSingleSignOnExtension resource type</span></span>

<span data-ttu-id="9818c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9818c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9818c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9818c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9818c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9818c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9818c-107">Представляет один профиль расширения Sign-On для типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="9818c-107">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="9818c-108">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="9818c-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9818c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9818c-109">Properties</span></span>
|<span data-ttu-id="9818c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9818c-110">Property</span></span>|<span data-ttu-id="9818c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9818c-111">Type</span></span>|<span data-ttu-id="9818c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9818c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9818c-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="9818c-113">extensionIdentifier</span></span>|<span data-ttu-id="9818c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="9818c-114">String</span></span>|<span data-ttu-id="9818c-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="9818c-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="9818c-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="9818c-116">teamIdentifier</span></span>|<span data-ttu-id="9818c-117">Строка</span><span class="sxs-lookup"><span data-stu-id="9818c-117">String</span></span>|<span data-ttu-id="9818c-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="9818c-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="9818c-119">домена</span><span class="sxs-lookup"><span data-stu-id="9818c-119">domains</span></span>|<span data-ttu-id="9818c-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9818c-120">String collection</span></span>|<span data-ttu-id="9818c-121">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="9818c-121">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="9818c-122">область</span><span class="sxs-lookup"><span data-stu-id="9818c-122">realm</span></span>|<span data-ttu-id="9818c-123">Строка</span><span class="sxs-lookup"><span data-stu-id="9818c-123">String</span></span>|<span data-ttu-id="9818c-124">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="9818c-124">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="9818c-125">построения</span><span class="sxs-lookup"><span data-stu-id="9818c-125">configurations</span></span>|<span data-ttu-id="9818c-126">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9818c-126">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="9818c-127">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="9818c-127">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="9818c-128">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9818c-128">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9818c-129">Связи</span><span class="sxs-lookup"><span data-stu-id="9818c-129">Relationships</span></span>
<span data-ttu-id="9818c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="9818c-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9818c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9818c-131">JSON Representation</span></span>
<span data-ttu-id="9818c-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9818c-132">Here is a JSON representation of the resource.</span></span>
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





