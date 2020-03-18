---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd959b3019a6bd4ce553b53a70042fffd5c9b277
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790540"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="6d188-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="6d188-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="6d188-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d188-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d188-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d188-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d188-106">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="6d188-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="6d188-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d188-107">Properties</span></span>
|<span data-ttu-id="6d188-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d188-108">Property</span></span>|<span data-ttu-id="6d188-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6d188-109">Type</span></span>|<span data-ttu-id="6d188-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d188-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d188-111">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="6d188-111">allowedAppsList</span></span>|<span data-ttu-id="6d188-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d188-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6d188-113">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="6d188-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="6d188-114">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d188-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="6d188-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d188-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d188-116">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="6d188-116">allowedUrls</span></span>|<span data-ttu-id="6d188-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d188-117">String collection</span></span>|<span data-ttu-id="6d188-118">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="6d188-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="6d188-119">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="6d188-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="6d188-120">displayName</span><span class="sxs-lookup"><span data-stu-id="6d188-120">displayName</span></span>|<span data-ttu-id="6d188-121">String</span><span class="sxs-lookup"><span data-stu-id="6d188-121">String</span></span>|<span data-ttu-id="6d188-122">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d188-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="6d188-123">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="6d188-123">kerberosPrincipalName</span></span>|<span data-ttu-id="6d188-124">String</span><span class="sxs-lookup"><span data-stu-id="6d188-124">String</span></span>|<span data-ttu-id="6d188-125">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="6d188-125">A Kerberos principal name.</span></span> <span data-ttu-id="6d188-126">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="6d188-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="6d188-127">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="6d188-127">kerberosRealm</span></span>|<span data-ttu-id="6d188-128">String</span><span class="sxs-lookup"><span data-stu-id="6d188-128">String</span></span>|<span data-ttu-id="6d188-129">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="6d188-129">A Kerberos realm name.</span></span> <span data-ttu-id="6d188-130">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="6d188-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d188-131">Связи</span><span class="sxs-lookup"><span data-stu-id="6d188-131">Relationships</span></span>
<span data-ttu-id="6d188-132">Нет</span><span class="sxs-lookup"><span data-stu-id="6d188-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d188-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d188-133">JSON Representation</span></span>
<span data-ttu-id="6d188-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d188-134">Here is a JSON representation of the resource.</span></span>
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



