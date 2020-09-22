---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6206dbc62fa8ae9ff0dee4d47bec30ce4ae99ae0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003642"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="57947-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="57947-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="57947-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57947-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57947-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57947-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57947-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57947-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57947-107">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="57947-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="57947-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="57947-108">Properties</span></span>
|<span data-ttu-id="57947-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="57947-109">Property</span></span>|<span data-ttu-id="57947-110">Тип</span><span class="sxs-lookup"><span data-stu-id="57947-110">Type</span></span>|<span data-ttu-id="57947-111">Описание</span><span class="sxs-lookup"><span data-stu-id="57947-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57947-112">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="57947-112">allowedAppsList</span></span>|<span data-ttu-id="57947-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="57947-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="57947-114">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="57947-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="57947-115">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="57947-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="57947-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="57947-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="57947-117">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="57947-117">allowedUrls</span></span>|<span data-ttu-id="57947-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57947-118">String collection</span></span>|<span data-ttu-id="57947-119">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="57947-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="57947-120">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="57947-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="57947-121">displayName</span><span class="sxs-lookup"><span data-stu-id="57947-121">displayName</span></span>|<span data-ttu-id="57947-122">String</span><span class="sxs-lookup"><span data-stu-id="57947-122">String</span></span>|<span data-ttu-id="57947-123">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="57947-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="57947-124">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="57947-124">kerberosPrincipalName</span></span>|<span data-ttu-id="57947-125">String</span><span class="sxs-lookup"><span data-stu-id="57947-125">String</span></span>|<span data-ttu-id="57947-126">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="57947-126">A Kerberos principal name.</span></span> <span data-ttu-id="57947-127">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="57947-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="57947-128">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="57947-128">kerberosRealm</span></span>|<span data-ttu-id="57947-129">String</span><span class="sxs-lookup"><span data-stu-id="57947-129">String</span></span>|<span data-ttu-id="57947-130">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="57947-130">A Kerberos realm name.</span></span> <span data-ttu-id="57947-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="57947-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57947-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="57947-132">Relationships</span></span>
<span data-ttu-id="57947-133">Нет</span><span class="sxs-lookup"><span data-stu-id="57947-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57947-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57947-134">JSON Representation</span></span>
<span data-ttu-id="57947-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57947-135">Here is a JSON representation of the resource.</span></span>
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






