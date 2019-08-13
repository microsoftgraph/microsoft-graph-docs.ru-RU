---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7395b17e9ac8c266f4eb1db676ce7190dbc6b1a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356839"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="206a1-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="206a1-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="206a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="206a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="206a1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="206a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="206a1-106">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="206a1-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="206a1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="206a1-107">Properties</span></span>
|<span data-ttu-id="206a1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="206a1-108">Property</span></span>|<span data-ttu-id="206a1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="206a1-109">Type</span></span>|<span data-ttu-id="206a1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="206a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="206a1-111">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="206a1-111">allowedAppsList</span></span>|<span data-ttu-id="206a1-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="206a1-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="206a1-113">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="206a1-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="206a1-114">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="206a1-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="206a1-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="206a1-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="206a1-116">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="206a1-116">allowedUrls</span></span>|<span data-ttu-id="206a1-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="206a1-117">String collection</span></span>|<span data-ttu-id="206a1-118">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="206a1-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="206a1-119">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="206a1-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="206a1-120">displayName</span><span class="sxs-lookup"><span data-stu-id="206a1-120">displayName</span></span>|<span data-ttu-id="206a1-121">String</span><span class="sxs-lookup"><span data-stu-id="206a1-121">String</span></span>|<span data-ttu-id="206a1-122">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="206a1-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="206a1-123">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="206a1-123">kerberosPrincipalName</span></span>|<span data-ttu-id="206a1-124">String</span><span class="sxs-lookup"><span data-stu-id="206a1-124">String</span></span>|<span data-ttu-id="206a1-125">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="206a1-125">A Kerberos principal name.</span></span> <span data-ttu-id="206a1-126">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="206a1-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="206a1-127">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="206a1-127">kerberosRealm</span></span>|<span data-ttu-id="206a1-128">String</span><span class="sxs-lookup"><span data-stu-id="206a1-128">String</span></span>|<span data-ttu-id="206a1-129">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="206a1-129">A Kerberos realm name.</span></span> <span data-ttu-id="206a1-130">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="206a1-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="206a1-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="206a1-131">Relationships</span></span>
<span data-ttu-id="206a1-132">Нет</span><span class="sxs-lookup"><span data-stu-id="206a1-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="206a1-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="206a1-133">JSON Representation</span></span>
<span data-ttu-id="206a1-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="206a1-134">Here is a JSON representation of the resource.</span></span>
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



