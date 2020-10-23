---
title: Тип ресурса Иосредиректсинглесигнонекстенсион
description: Представляет тип перенаправления с одним Sign-Onным профилем расширения для устройств с iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed328be986939da8d4da8866e2c6c238fb755e46
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705696"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="0d93d-103">Тип ресурса Иосредиректсинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="0d93d-103">iosRedirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="0d93d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d93d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d93d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d93d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d93d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d93d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d93d-107">Представляет тип перенаправления с одним Sign-Onным профилем расширения для устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="0d93d-107">Represents a Redirect-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="0d93d-108">Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="0d93d-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d93d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d93d-109">Properties</span></span>
|<span data-ttu-id="0d93d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d93d-110">Property</span></span>|<span data-ttu-id="0d93d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0d93d-111">Type</span></span>|<span data-ttu-id="0d93d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0d93d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d93d-113">екстенсионидентифиер</span><span class="sxs-lookup"><span data-stu-id="0d93d-113">extensionIdentifier</span></span>|<span data-ttu-id="0d93d-114">Строка</span><span class="sxs-lookup"><span data-stu-id="0d93d-114">String</span></span>|<span data-ttu-id="0d93d-115">Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="0d93d-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="0d93d-116">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="0d93d-116">teamIdentifier</span></span>|<span data-ttu-id="0d93d-117">Строка</span><span class="sxs-lookup"><span data-stu-id="0d93d-117">String</span></span>|<span data-ttu-id="0d93d-118">Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="0d93d-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="0d93d-119">построения</span><span class="sxs-lookup"><span data-stu-id="0d93d-119">configurations</span></span>|<span data-ttu-id="0d93d-120">Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0d93d-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="0d93d-121">Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0d93d-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="0d93d-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0d93d-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0d93d-123">урлпрефиксес</span><span class="sxs-lookup"><span data-stu-id="0d93d-123">urlPrefixes</span></span>|<span data-ttu-id="0d93d-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d93d-124">String collection</span></span>|<span data-ttu-id="0d93d-125">Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход.</span><span class="sxs-lookup"><span data-stu-id="0d93d-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="0d93d-126">URL-адреса должны начинаться с http://или https://.</span><span class="sxs-lookup"><span data-stu-id="0d93d-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="0d93d-127">Все префиксы URL-адреса должны быть уникальными для всех профилей.</span><span class="sxs-lookup"><span data-stu-id="0d93d-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d93d-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0d93d-128">Relationships</span></span>
<span data-ttu-id="0d93d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0d93d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d93d-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d93d-130">JSON Representation</span></span>
<span data-ttu-id="0d93d-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d93d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```





