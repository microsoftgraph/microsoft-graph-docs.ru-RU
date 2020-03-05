---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f35240243b94a2abdc817823b70d53a64b43dca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529855"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="278a2-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="278a2-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="278a2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="278a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="278a2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="278a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="278a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="278a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="278a2-107">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="278a2-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="278a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="278a2-108">Properties</span></span>
|<span data-ttu-id="278a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="278a2-109">Property</span></span>|<span data-ttu-id="278a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="278a2-110">Type</span></span>|<span data-ttu-id="278a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="278a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="278a2-112">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="278a2-112">allowedAppsList</span></span>|<span data-ttu-id="278a2-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="278a2-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="278a2-114">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="278a2-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="278a2-115">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="278a2-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="278a2-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="278a2-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="278a2-117">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="278a2-117">allowedUrls</span></span>|<span data-ttu-id="278a2-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="278a2-118">String collection</span></span>|<span data-ttu-id="278a2-119">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="278a2-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="278a2-120">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="278a2-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="278a2-121">displayName</span><span class="sxs-lookup"><span data-stu-id="278a2-121">displayName</span></span>|<span data-ttu-id="278a2-122">String</span><span class="sxs-lookup"><span data-stu-id="278a2-122">String</span></span>|<span data-ttu-id="278a2-123">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="278a2-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="278a2-124">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="278a2-124">kerberosPrincipalName</span></span>|<span data-ttu-id="278a2-125">String</span><span class="sxs-lookup"><span data-stu-id="278a2-125">String</span></span>|<span data-ttu-id="278a2-126">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="278a2-126">A Kerberos principal name.</span></span> <span data-ttu-id="278a2-127">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="278a2-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="278a2-128">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="278a2-128">kerberosRealm</span></span>|<span data-ttu-id="278a2-129">String</span><span class="sxs-lookup"><span data-stu-id="278a2-129">String</span></span>|<span data-ttu-id="278a2-130">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="278a2-130">A Kerberos realm name.</span></span> <span data-ttu-id="278a2-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="278a2-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="278a2-132">Связи</span><span class="sxs-lookup"><span data-stu-id="278a2-132">Relationships</span></span>
<span data-ttu-id="278a2-133">Нет</span><span class="sxs-lookup"><span data-stu-id="278a2-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="278a2-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="278a2-134">JSON Representation</span></span>
<span data-ttu-id="278a2-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="278a2-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```



