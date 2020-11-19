---
title: Тип ресурса Макоскредентиалсинглесигнонекстенсион
description: Представляет один профиль расширения учетных данных с Sign-On для устройств macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 154718699b15187cad409538d90912b4cfdf7708
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268708"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a><span data-ttu-id="4c021-103">Тип ресурса Макоскредентиалсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="4c021-103">macOSCredentialSingleSignOnExtension resource type</span></span>

<span data-ttu-id="4c021-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c021-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c021-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c021-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c021-107">Представляет один профиль расширения учетных данных с Sign-On для устройств macOS.</span><span class="sxs-lookup"><span data-stu-id="4c021-107">Represents a Credential-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="4c021-108">Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="4c021-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c021-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c021-109">Properties</span></span>
|<span data-ttu-id="4c021-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c021-110">Property</span></span>|<span data-ttu-id="4c021-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4c021-111">Type</span></span>|<span data-ttu-id="4c021-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4c021-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c021-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="4c021-113">extensionIdentifier</span></span>|<span data-ttu-id="4c021-114">String</span><span class="sxs-lookup"><span data-stu-id="4c021-114">String</span></span>|<span data-ttu-id="4c021-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4c021-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4c021-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="4c021-116">teamIdentifier</span></span>|<span data-ttu-id="4c021-117">String</span><span class="sxs-lookup"><span data-stu-id="4c021-117">String</span></span>|<span data-ttu-id="4c021-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4c021-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="4c021-119">домена</span><span class="sxs-lookup"><span data-stu-id="4c021-119">domains</span></span>|<span data-ttu-id="4c021-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4c021-120">String collection</span></span>|<span data-ttu-id="4c021-121">Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="4c021-121">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="4c021-122">область</span><span class="sxs-lookup"><span data-stu-id="4c021-122">realm</span></span>|<span data-ttu-id="4c021-123">String</span><span class="sxs-lookup"><span data-stu-id="4c021-123">String</span></span>|<span data-ttu-id="4c021-124">Получает или задает имя области для этого профиля, заданное с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="4c021-124">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="4c021-125">построения</span><span class="sxs-lookup"><span data-stu-id="4c021-125">configurations</span></span>|<span data-ttu-id="4c021-126">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4c021-126">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="4c021-127">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4c021-127">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="4c021-128">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4c021-128">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c021-129">Связи</span><span class="sxs-lookup"><span data-stu-id="4c021-129">Relationships</span></span>
<span data-ttu-id="4c021-130">Нет</span><span class="sxs-lookup"><span data-stu-id="4c021-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c021-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c021-131">JSON Representation</span></span>
<span data-ttu-id="4c021-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c021-132">Here is a JSON representation of the resource.</span></span>
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




