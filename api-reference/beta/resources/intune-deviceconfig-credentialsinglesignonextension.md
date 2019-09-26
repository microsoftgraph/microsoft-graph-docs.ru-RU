---
title: Тип ресурса Кредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с типом учетных данных.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 588dc5e92a46e7361ca083570a4b92d0f3fbff62
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201317"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="ed35f-103">Тип ресурса Кредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="ed35f-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="ed35f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed35f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed35f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed35f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed35f-106">Представляет профиль расширения единого входа с типом учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ed35f-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="ed35f-107">Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="ed35f-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed35f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed35f-108">Properties</span></span>
|<span data-ttu-id="ed35f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed35f-109">Property</span></span>|<span data-ttu-id="ed35f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed35f-110">Type</span></span>|<span data-ttu-id="ed35f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed35f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed35f-112">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="ed35f-112">extensionIdentifier</span></span>|<span data-ttu-id="ed35f-113">String.</span><span class="sxs-lookup"><span data-stu-id="ed35f-113">String</span></span>|<span data-ttu-id="ed35f-114">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ed35f-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ed35f-115">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="ed35f-115">teamIdentifier</span></span>|<span data-ttu-id="ed35f-116">String.</span><span class="sxs-lookup"><span data-stu-id="ed35f-116">String</span></span>|<span data-ttu-id="ed35f-117">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ed35f-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ed35f-118">домена</span><span class="sxs-lookup"><span data-stu-id="ed35f-118">domains</span></span>|<span data-ttu-id="ed35f-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ed35f-119">String collection</span></span>|<span data-ttu-id="ed35f-120">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="ed35f-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="ed35f-121">область</span><span class="sxs-lookup"><span data-stu-id="ed35f-121">realm</span></span>|<span data-ttu-id="ed35f-122">String.</span><span class="sxs-lookup"><span data-stu-id="ed35f-122">String</span></span>|<span data-ttu-id="ed35f-123">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="ed35f-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="ed35f-124">построения</span><span class="sxs-lookup"><span data-stu-id="ed35f-124">configurations</span></span>|<span data-ttu-id="ed35f-125">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ed35f-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="ed35f-126">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ed35f-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="ed35f-127">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ed35f-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed35f-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="ed35f-128">Relationships</span></span>
<span data-ttu-id="ed35f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ed35f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed35f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed35f-130">JSON Representation</span></span>
<span data-ttu-id="ed35f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed35f-131">Here is a JSON representation of the resource.</span></span>
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



