---
title: тип enum configurationManagerActionDeliveryStatus
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cda8bbb7f52898ddd042b8cba88b204907bfe9edff006510a61b6b36c7db66eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239415"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>тип enum configurationManagerActionDeliveryStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние доставки действия устройства Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Ожидание доставки действия в ConfigurationManager|
|pendingDelivery|1 |Ожидание доставки действия в ConfigurationManager|
|deliveredToConnectorService|2|Действие отправляется в службу Connector ConfigurationManager (облако)|
|failedToDeliverToConnectorService|3 |Не удалось отправить действие в службу Connector ConfigurationManager (облако)|
|deliveredToOnPremisesServer|4 |Действие доставляется на сервер ConfigurationManager на предварительном сервере|




