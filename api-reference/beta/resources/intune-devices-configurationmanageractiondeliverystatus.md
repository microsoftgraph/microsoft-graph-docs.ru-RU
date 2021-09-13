---
title: тип enum configurationManagerActionDeliveryStatus
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e776d03e4d785191ff3463bae125d786250ee22d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111007"
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
|pendingDelivery|1|Ожидание доставки действия в ConfigurationManager|
|deliveredToConnectorService|2|Действие отправляется в службу Connector ConfigurationManager (облако)|
|failedToDeliverToConnectorService|3|Не удалось отправить действие в службу Connector ConfigurationManager (облако)|
|deliveredToOnPremisesServer|4 |Действие доставляется на сервер ConfigurationManager на предварительном сервере|



