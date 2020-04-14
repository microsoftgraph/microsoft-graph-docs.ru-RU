---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f43f5feea67f9f94a8aa5f9179add26deb84ee6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440191"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="3f59d-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="3f59d-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="3f59d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f59d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f59d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f59d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f59d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f59d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f59d-107">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="3f59d-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="3f59d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f59d-108">Properties</span></span>
|<span data-ttu-id="3f59d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f59d-109">Property</span></span>|<span data-ttu-id="3f59d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f59d-110">Type</span></span>|<span data-ttu-id="3f59d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f59d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f59d-112">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="3f59d-112">allowedAppsList</span></span>|<span data-ttu-id="3f59d-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f59d-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3f59d-114">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="3f59d-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="3f59d-115">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3f59d-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="3f59d-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3f59d-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3f59d-117">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="3f59d-117">allowedUrls</span></span>|<span data-ttu-id="3f59d-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f59d-118">String collection</span></span>|<span data-ttu-id="3f59d-119">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="3f59d-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="3f59d-120">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="3f59d-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="3f59d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="3f59d-121">displayName</span></span>|<span data-ttu-id="3f59d-122">String</span><span class="sxs-lookup"><span data-stu-id="3f59d-122">String</span></span>|<span data-ttu-id="3f59d-123">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="3f59d-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="3f59d-124">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="3f59d-124">kerberosPrincipalName</span></span>|<span data-ttu-id="3f59d-125">String</span><span class="sxs-lookup"><span data-stu-id="3f59d-125">String</span></span>|<span data-ttu-id="3f59d-126">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="3f59d-126">A Kerberos principal name.</span></span> <span data-ttu-id="3f59d-127">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="3f59d-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="3f59d-128">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="3f59d-128">kerberosRealm</span></span>|<span data-ttu-id="3f59d-129">String</span><span class="sxs-lookup"><span data-stu-id="3f59d-129">String</span></span>|<span data-ttu-id="3f59d-130">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="3f59d-130">A Kerberos realm name.</span></span> <span data-ttu-id="3f59d-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="3f59d-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f59d-132">Связи</span><span class="sxs-lookup"><span data-stu-id="3f59d-132">Relationships</span></span>
<span data-ttu-id="3f59d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3f59d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f59d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f59d-134">JSON Representation</span></span>
<span data-ttu-id="3f59d-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f59d-135">Here is a JSON representation of the resource.</span></span>
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



