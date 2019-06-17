---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11875bb07b87cf8c9415660f5961dafa73f54f57
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995618"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="55b10-103">Тип ресурса Иоссинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="55b10-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="55b10-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b10-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55b10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b10-106">Параметры проверки подлинности Kerberos для iOS для единого входа</span><span class="sxs-lookup"><span data-stu-id="55b10-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="55b10-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55b10-107">Properties</span></span>
|<span data-ttu-id="55b10-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b10-108">Property</span></span>|<span data-ttu-id="55b10-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55b10-109">Type</span></span>|<span data-ttu-id="55b10-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55b10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b10-111">Алловедаппслист</span><span class="sxs-lookup"><span data-stu-id="55b10-111">allowedAppsList</span></span>|<span data-ttu-id="55b10-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="55b10-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="55b10-113">Список идентификаторов приложений, которым разрешено использовать это имя для входа.</span><span class="sxs-lookup"><span data-stu-id="55b10-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="55b10-114">Если это поле опущено, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="55b10-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="55b10-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="55b10-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="55b10-116">Алловедурлс</span><span class="sxs-lookup"><span data-stu-id="55b10-116">allowedUrls</span></span>|<span data-ttu-id="55b10-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="55b10-117">String collection</span></span>|<span data-ttu-id="55b10-118">Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа.</span><span class="sxs-lookup"><span data-stu-id="55b10-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="55b10-119">При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="55b10-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="55b10-120">displayName</span><span class="sxs-lookup"><span data-stu-id="55b10-120">displayName</span></span>|<span data-ttu-id="55b10-121">String</span><span class="sxs-lookup"><span data-stu-id="55b10-121">String</span></span>|<span data-ttu-id="55b10-122">Отображаемое имя параметров входа, отображаемое на принимающем устройстве.</span><span class="sxs-lookup"><span data-stu-id="55b10-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="55b10-123">КербероспринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="55b10-123">kerberosPrincipalName</span></span>|<span data-ttu-id="55b10-124">String</span><span class="sxs-lookup"><span data-stu-id="55b10-124">String</span></span>|<span data-ttu-id="55b10-125">Имя субъекта Kerberos.</span><span class="sxs-lookup"><span data-stu-id="55b10-125">A Kerberos principal name.</span></span> <span data-ttu-id="55b10-126">Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="55b10-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="55b10-127">Керберосреалм</span><span class="sxs-lookup"><span data-stu-id="55b10-127">kerberosRealm</span></span>|<span data-ttu-id="55b10-128">String</span><span class="sxs-lookup"><span data-stu-id="55b10-128">String</span></span>|<span data-ttu-id="55b10-129">Имя области Kerberos.</span><span class="sxs-lookup"><span data-stu-id="55b10-129">A Kerberos realm name.</span></span> <span data-ttu-id="55b10-130">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="55b10-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55b10-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="55b10-131">Relationships</span></span>
<span data-ttu-id="55b10-132">Нет</span><span class="sxs-lookup"><span data-stu-id="55b10-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b10-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55b10-133">JSON Representation</span></span>
<span data-ttu-id="55b10-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55b10-134">Here is a JSON representation of the resource.</span></span>
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





