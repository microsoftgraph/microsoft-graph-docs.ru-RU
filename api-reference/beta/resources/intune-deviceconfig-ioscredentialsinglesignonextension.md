---
title: Тип ресурса Иоскредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с использованием учетных данных для устройств с iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cf6f3202abb5fce499a842a03aae189fc1572141
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791662"
---
# <a name="ioscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="27bf3-103">Тип ресурса Иоскредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="27bf3-103">iosCredentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="27bf3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27bf3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27bf3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27bf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27bf3-106">Представляет профиль расширения единого входа с использованием учетных данных для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="27bf3-106">Represents a Credential-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="27bf3-107">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="27bf3-107">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27bf3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="27bf3-108">Properties</span></span>
|<span data-ttu-id="27bf3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="27bf3-109">Property</span></span>|<span data-ttu-id="27bf3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="27bf3-110">Type</span></span>|<span data-ttu-id="27bf3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27bf3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27bf3-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="27bf3-112">extensionIdentifier</span></span>|<span data-ttu-id="27bf3-113">String</span><span class="sxs-lookup"><span data-stu-id="27bf3-113">String</span></span>|<span data-ttu-id="27bf3-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="27bf3-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="27bf3-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="27bf3-115">teamIdentifier</span></span>|<span data-ttu-id="27bf3-116">String</span><span class="sxs-lookup"><span data-stu-id="27bf3-116">String</span></span>|<span data-ttu-id="27bf3-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="27bf3-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="27bf3-118">домена</span><span class="sxs-lookup"><span data-stu-id="27bf3-118">domains</span></span>|<span data-ttu-id="27bf3-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27bf3-119">String collection</span></span>|<span data-ttu-id="27bf3-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="27bf3-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="27bf3-121">область</span><span class="sxs-lookup"><span data-stu-id="27bf3-121">realm</span></span>|<span data-ttu-id="27bf3-122">String</span><span class="sxs-lookup"><span data-stu-id="27bf3-122">String</span></span>|<span data-ttu-id="27bf3-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="27bf3-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="27bf3-124">построения</span><span class="sxs-lookup"><span data-stu-id="27bf3-124">configurations</span></span>|<span data-ttu-id="27bf3-125">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="27bf3-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="27bf3-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="27bf3-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="27bf3-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="27bf3-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27bf3-128">Связи</span><span class="sxs-lookup"><span data-stu-id="27bf3-128">Relationships</span></span>
<span data-ttu-id="27bf3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="27bf3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27bf3-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27bf3-130">JSON Representation</span></span>
<span data-ttu-id="27bf3-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27bf3-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCredentialSingleSignOnExtension",
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



