---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20c6cabbd5f18349058c68136052c8d56894dccc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728565"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="42112-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="42112-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="42112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42112-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42112-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42112-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42112-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42112-107">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="42112-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="42112-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="42112-108">Properties</span></span>
|<span data-ttu-id="42112-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="42112-109">Property</span></span>|<span data-ttu-id="42112-110">Тип</span><span class="sxs-lookup"><span data-stu-id="42112-110">Type</span></span>|<span data-ttu-id="42112-111">Описание</span><span class="sxs-lookup"><span data-stu-id="42112-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42112-112">алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="42112-112">allowedAppsList</span></span>|<span data-ttu-id="42112-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="42112-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="42112-114">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="42112-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="42112-115">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="42112-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="42112-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="42112-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="42112-117">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="42112-117">allowedUrls</span></span>|<span data-ttu-id="42112-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42112-118">String collection</span></span>|<span data-ttu-id="42112-119">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="42112-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="42112-120">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="42112-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="42112-121">displayName</span><span class="sxs-lookup"><span data-stu-id="42112-121">displayName</span></span>|<span data-ttu-id="42112-122">Строка</span><span class="sxs-lookup"><span data-stu-id="42112-122">String</span></span>|<span data-ttu-id="42112-123">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="42112-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="42112-124">кербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="42112-124">kerberosPrincipalName</span></span>|<span data-ttu-id="42112-125">Строка</span><span class="sxs-lookup"><span data-stu-id="42112-125">String</span></span>|<span data-ttu-id="42112-126">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="42112-126">A Kerberos principal name.</span></span> <span data-ttu-id="42112-127">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="42112-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="42112-128">керберосреалм</span><span class="sxs-lookup"><span data-stu-id="42112-128">kerberosRealm</span></span>|<span data-ttu-id="42112-129">Строка</span><span class="sxs-lookup"><span data-stu-id="42112-129">String</span></span>|<span data-ttu-id="42112-130">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="42112-130">A Kerberos realm name.</span></span> <span data-ttu-id="42112-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="42112-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42112-132">Связи</span><span class="sxs-lookup"><span data-stu-id="42112-132">Relationships</span></span>
<span data-ttu-id="42112-133">Нет</span><span class="sxs-lookup"><span data-stu-id="42112-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42112-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42112-134">JSON Representation</span></span>
<span data-ttu-id="42112-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42112-135">Here is a JSON representation of the resource.</span></span>
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





